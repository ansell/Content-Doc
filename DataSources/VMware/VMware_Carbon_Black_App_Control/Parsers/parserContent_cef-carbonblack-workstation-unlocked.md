#### Parser Content
```Java
{
Name = cef-carbonblack-workstation-unlocked
  Vendor = VMware
  Product = VMware Carbon Black App Control
  Lms = ArcSight
  DataType = "workstation-unlocked"
  TimeFormat = "epoch"
  Conditions = [ """|Carbon Black|Protection|""", """Event[00000008] Type[SessionUnlock]""" ]
  Fields = [
    """\Wrt=({time}\d+)""",
    """\Wdvc=({host}[a-fA-F:\d.]+)""",
    """\Wdvchost=({host}[\w\-.]+)""",
    """\Wdhost=(({domain}[^\\]+)\\+)?({dest_host}[^\\\s]+)""",
    """\Wdst=({dest_ip}[a-fA-F:\d.]+)""",
    """\Wduser=(({domain}[^\\]+)\\+)?({user}[^\\\s]+)""",
    """\WEvent\[({event_code}\d+)\]\s*Type\[Session"""
  ]
}
```