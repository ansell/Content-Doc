#### Parser Content
```Java
{
Name = cef-defender-atp-member-added
  DataType = "windows-member-added"
  Conditions = ["""CEF:""", """|SkyFormation Cloud Apps Security|""", """requestClientApplication=""", """AdvancedHunting-DeviceEvents""","""UserAccountAddedToLocalGroup"""]
  Fields = ${MicrosoftParserTemplates.cef-defender-atp.Fields}[
  """"LogonId":(null|"({logon_id}[^"]+))""",
  """AccountDomain":"({group_domain}[^"]+)"""
]
}
```