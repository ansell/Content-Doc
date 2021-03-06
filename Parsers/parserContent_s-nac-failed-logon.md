#### Parser Content
```Java
{
Name = s-nac-failed-logon
  Vendor = Cisco
  Product = Cisco ISE
  Lms = Splunk
  DataType = "nac-failed-logon"
  TimeFormat = "yyyy-MM-dd HH:mm:ss"
  Conditions = [ "CISE_Failed_Attempts", "since user has entered the wrong password" ]
  Fields = [
    """exabeam_host=({host}[^\s]+)""",
    """({host}[\w\-.]+)\s+CISE_Failed_Attempts""",
    """\d+\s+({time}\d\d\d\d\-\d\d\-\d\d \d+:\d+:\d+)""",
    """, UserName=(({user_type}host)\/)?(({domain}[^\s\\]+)\\+)?(({user_email}[^,@]+@[^,@]+)|({user}[^,]+))""",
    """, Calling-Station-ID=({dest_host}[^,]+)""",
    """, Called-Station-ID=({src_host}[^,]+):({ssid}[^,]+)""",
    """, AD-Host-Resolved-Identities=({dest_host}[^@,]+)""",
    """, AD-Host-Resolved-Identities=({computer_name}[^@,]+)""",
    """, (NetworkDeviceName|NetworkDeviceProfileName)=({network}[^,]+)""",
    """, Device IP Address=({auth_server}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})""",
    """, Device IP Address=({dest_ip}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})""",
    """, Framed-IP-Address=({dest_ip}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})""",
    """, DestinationIPAddress=({dest_ip}[a-fA-F\d.:]+)""",
    """, NetworkDeviceGroups=Location#All Locations#({location}[^,]+)""",
    """, FailureReason=({result_code}\d+)""",
    """, FailureReason=\d+ ({failure_reason}[^,]+)""",
    """(?i)(MacAddress)=({mac_address}[^,\s]+),""",
    """, SSID=({ssid}[^,]+)""",
    """, AuthenticationIdentityStore=({auth_server}[^,]+)""",
  ]
}
```