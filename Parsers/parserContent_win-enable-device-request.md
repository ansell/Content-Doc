#### Parser Content
```Java
{
Name = win-enable-device-request
  DataType = "usb-activity"
  Conditions = [ """A request was made to enable a device.""" ]
  Fields = ${WinParserTemplates.d-xml-windows-device.Fields} [
    """({event_code}6421)""",
    """>({event_code}6421)<\/EventID>"""
    """({event_name}A request was made to enable a device.)"""
  ]
}
```