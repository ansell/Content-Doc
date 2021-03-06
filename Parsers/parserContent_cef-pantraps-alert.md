#### Parser Content
```Java
{
Name = cef-pantraps-alert
  Vendor = Palo Alto Networks
  Product = Traps
  Lms = Splunk
  DataType = "alert"
  TimeFormat = "MMM dd yyyy HH:mm:ss"
  Conditions = [ """|Palo Alto Networks|Traps Agent|""","""Prevention Key:""" ]
  Fields = [
    """exabeam_host=({host}[\w.\-]+)""",
    """\d\d:\d\d:\d\d ({host}[^\s]+)\sCEF""",
    """(devTime|rt)=({time}\w+ \d+ \d\d\d\d \d\d:\d\d:\d\d)""",
    """duser=(({domain}[^\\]+)\\)?(?: |({user}.+?))\s*\w+=""",
    """dhost=(?: |({src_host}.+?))\s*\w+=""",
    """\|Palo Alto Networks\|([^|]+\|){2}({alert_name}[^|]+)""",
    """\|Palo Alto Networks\|([^|]+\|){4}({alert_severity}[^|]+)""",
    """(subtype|cs2)=(?: |({alert_type}.+?))\s*\w+=""",
    """Prevention Key: (?: |({alert_id}.+?))\s*($|\w+=)""",
    """deviceProcessName=(?: |({malware_url}.+?))\s*\w+=""",
    """msg=(?: |({additional_info}.+?))(\.|:)"""
  ]
  SOAR {
    IncidentType = "malware"
    DupFields = ["time->startedDate", "vendor->source", "rawLog->sourceInfo", "alert_name->malwareName", "alert_severity->sourceSeverity", "alert_id->sourceId", "src_host->malwareVictimHost", "alert_type->description", "malware_url->malwareAttackerUrl"]
    NameTemplate = """Palo Alto Alert ${alert_name} found"""
    ProjectName = "SOC"
    EntityFields = [
      {EntityType="device", Name="src_address", Fields=["src_host->host_name"]}
```