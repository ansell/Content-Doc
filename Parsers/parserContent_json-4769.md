#### Parser Content
```Java
{
Name = json-4769
    Vendor = Microsoft
    Product = Microsoft Windows
    Lms = Direct
    DataType = "windows-4769"
    TimeFormat = "yyyy-MM-dd'T'HH:mm:ss"
    Conditions = ["""4769""", """"TransmittedServices":""""]
    Fields = [
      """({event_name}A Kerberos service ticket was requested)""",
      """"EventTime":"({time}\d\d\d\d-\d\d-\d\d \d\d:\d\d:\d\d)""",
      """"EventReceivedTime":\s*({time}\d+)""",
      """"timestamp":\s*({time}\d+)""",
      """\s({time}\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d.\d\d\dZ)\s[^\s]+\sSkyformation""",
      """"+created"+:"+({time}[^"]+)""",
      """"TimeCreated"+:"+({time}\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d)""",
      """"Computer"+:"+({host}[^"]+)""""
      """"+(?:winlog\.)?computer_name"+:"+({host}[^"]+)""",
      """"(Hostname|MachineName)":"({host}[^"]*)""",
      """({event_code}4769)""",
      """"TargetUserName":"({user}[^@"]+)""",
      """"TargetDomainName":"({domain}[^."]+)""",
      """"ServiceName":"({dest_host}[^@"]+\$)"""",
      """"ServiceName":"({service_name}[^@"]+)"""",
      """"TicketOptions":"({ticket_options}[^"]+)""",
      """"TicketEncryptionType":"({ticket_encryption_type}[^"]+)""",
      """"IpAddress":"(::[\w]+:)?({src_ip}[a-fA-F:\d.]+)""",
      """"Status":"({result_code}[^"]+)"""
    ]
  }
```