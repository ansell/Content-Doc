#### Parser Content
```Java
{
Name = raw-5805
  Vendor = Microsoft
  Product = Microsoft Windows
  Lms = Direct
  DataType = "windows-failed-logon"
  TimeFormat = "yyyy-MM-dd'T'HH:mm:ss.SSSSSSSSSZ"
  Conditions = ["""NETLOGON""" , """The session setup from the computer""", """5805</EventID>""" ]
  Fields = [
    """SystemTime='({time}\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d\.\d+Z)""",
    """<EventID Qualifiers='0'>({event_code}5805)<\/EventID>""",
    """<Computer>({host}[^<]+)<\/Computer>""",
    """<Message>({additional_info}[^<]+)<\/Message>""",
    """ComputerName(:|=)\s*({host}[\w.-]+)""",
    """Event ID: ({event_code}\d+)""",
    """({event_name}The session setup from the computer ({src_host}[^\s]+)\sfailed to authenticate)""",
    """The following error occurred:\s+({failure_reason}[^<]+)\.<\/Message>"""
  ]
}
```