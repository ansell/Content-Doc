#### Parser Content
```Java
{
Name = s-json-4697
  Vendor = Microsoft
  Product = Microsoft Windows
  Lms = Splunk
  DataType = "windows-service-created"
  TimeFormat = "yyyy-MM-dd HH:mm:ss"
  Conditions = [ """"EventID":4697""", """A service was installed in the system""" ]
  Fields = [
    """"EventTime":"({time}\d\d\d\d-\d\d-\d\d \d\d:\d\d:\d\d)""",
    """({event_code}4697)""",
    """({event_name}A service was installed in the system)""",
    """"Hostname":"({host}[^"]+)"""",
    """"Keywords":({outcome}[^,]+),""",
    """"SubjectUserSid":"({user_sid}[^"]+)"""",
    """"SubjectUserName":"({user}[^"]+)"""",
    """"SubjectDomainName":"({domain}[^"]+)"""",
    """"SubjectLogonId":"({logon_id}[^"]+)"""",
    """"ServiceName":"({service_name}[^"]+)"""",
    """"ServiceFileName":"\s*(|({process}({directory}.*?[\\\/]+)?({process_name}[^\\\/]+?)))"""",
    """"ServiceType":"({service_type}[^"]+)"""",
    """"ServiceStartType":"({service_start_type}[^"]+)"""",
    """"ServiceAccount":"({account_domain}[^"]+)"""",
    """"ProcessID":({process_id}\d+)"""
  ]
  DupFields = [ "host->dest_host", "directory->process_directory" ]
}
```