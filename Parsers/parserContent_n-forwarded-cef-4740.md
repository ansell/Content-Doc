#### Parser Content
```Java
{
Name = n-forwarded-cef-4740
    Vendor = Microsoft
    Product = Microsoft Windows
    Lms = NitroCefSyslog
    DataType = "windows-account-lockout"
    TimeFormat = "epoch"
    Conditions = [ "|McAfee|ESM", "43-26304740"]
    Fields = [ """\|McAfee\|.+?\|43-2630({event_code}\d+)(0|1)\|""",
      """({event_name}A user account was locked out)""",
      """\srt=({time}\d+)""",
      """src=({host}[a-fA-F:\d.]+)""",
      """sntdom=({domain}[^\s]+)""",
      """shost=((|({domain}[^\\]*))\\+)?({src_host}[^\\\s]+)""",
      """duser=({caller_user}.+?)\s+\w+=""",
      """suser=({user}.+?)\s+\w+=""",
      """nitroSecurity_ID=({user_sid}[^\s]+)""",
      """nitroSource_Logon_ID=({logon_id}.+?)(\s|0\|)"""
    ]
    DupFields=[ "host->dest_host" ]
  }
```