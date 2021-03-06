#### Parser Content
```Java
{
Name = n-forwarded-cef-symantec-epp-alert
  Vendor = Symantec
  Product = Symantec Endpoint Protection
  Lms = NitroCefSyslog
  DataType = "alert"
  TimeFormat = "epoch"
  Conditions = [ "|McAfee|ESM", "|310-2771385440|" ]
  Fields = [ 
    """\srt=({time}\d+)""",
    """\|McAfee\|ESM\|.+?\|.+?\|({alert_type}.+?)\|""",
    """\|McAfee\|ESM\|.+?\|.+?\|.+?\|({alert_severity}.+?)\|""",
    """\sdeviceTranslatedAddress=({host}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})""",
    """\sexternalId=({alert_id}\d+)""",
    """\sshost=({src_host}.+?)\s+\w+=""",
    """\ssrc=({src_ip}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})""",
    """\snitroThreat_Name=({alert_name}.+?)\s+\w+=""",
    """\snitroDestination_Filename=({malware_url}.+?)\s+\w+="""
  ]
  SOAR {
    IncidentType = "malware"
    DupFields = ["time->startedDate", "vendor->source", "rawLog->sourceInfo", "alert_name->malwareName", "alert_severity->sourceSeverity", "alert_id->sourceId", "src_host->malwareVictimHost", "alert_type->description", "malware_url->malwareAttackerUrl"]
    NameTemplate = """Symantec Alert ${alert_name} found"""
    ProjectName = "SOC"
    EntityFields = [
      {EntityType="device", Name="src_address", Fields=["src_ip->ip_address", "src_host->host_name"]}
```