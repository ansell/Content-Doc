#### Parser Content
```Java
{
Name = cef-4720
  Vendor = Microsoft
  Product = Microsoft Windows
  Lms = ArcSight
  DataType = "windows-account-created"
  TimeFormat = "epoch"
  Conditions = [ """|Microsoft|Microsoft Windows|""","""|Microsoft-Windows-Security-Auditing:4720""" ]
  Fields = [ """exabeam_EventTime=({eventtime}\d+)""",
    """({event_name}A user account was created)""",
    """({event_code}4720)""",
    """\srt=({time}\d+)""",
    """\ssntdom=({domain}[^\s]+)""",
    """\ssuser=({user}.+?)\s+\w+=""",
    """\ssuid=({logon_id}[^\s]+)""",
    """\sdntdom=({account_domain}[^\s]+)""",
    """\sduser=({account_name}.+?)\s+\w+=""",
    """\sdvchost=({host}[^\s]+)""",
    """ad.New_,Account:Security_,ID=({account_id}[^\s]+)"""
  ]
   DupFields = ["host->dest_host"]
}
```