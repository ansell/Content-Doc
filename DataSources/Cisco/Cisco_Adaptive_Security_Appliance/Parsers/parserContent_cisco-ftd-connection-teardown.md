#### Parser Content
```Java
{
Name = cisco-ftd-connection-teardown
  Vendor = Cisco
  Product = Cisco Adaptive Security Appliance
  Lms = Direct
  DataType = "network-connection-stop"
  TimeFormat = "yyyy-MM-dd HH:mm:ss"
  Conditions = [ "%FTD-", "-30201", """: Teardown """, """ duration """ ]
  Fields = [
    """exabeam_time=({time}\d\d\d\d-\d\d-\d\d \d\d:\d\d:\d\d)""",
    """({host}[\w\-.]+)\s*:\s*%FTD-""",
    """%FTD-({priority}\d+)-({event_code}\d+)""",
    """({event_name}Teardown ({protocol}\w+) connection)""",
    """\sconnection\s+({connection_id}\d+)""",
    """\sfor\s+({src_interface}.+?):(({src_ip}(\d{1,3}\.){3}\d{1,3}|([A-Fa-f0-9%.]*:[A-Fa-f0-9%.:]+(th0)?))|({src_host}[^\s]+?))\/({src_port}\d+)""",
    """\sto\s+({dest_interface}.+?):(({dest_ip}(\d{1,3}\.){3}\d{1,3}|([A-Fa-f0-9%.]*:[A-Fa-f0-9%.:]+(th0)?))|({dest_host}[^\s]+?))\/({dest_port}\d+)""",
    """\sduration\s+({duration}\S+)\s+bytes\s+({bytes}\d+)(\s+({reason}[^\(]+[^\(\s]))?(\s+\(({user}.+?)\))?""",
    """%FTD-.*?\((({domain}[^\\\/]+)[\\\/]+)?({user}[^\\\/]+?)\)"""
  ]
  DupFields = [ "event_name->activity" ]
}
```