#### Parser Content
```Java
{
Name = cloudflare-app-activity
  Vendor = Cloudflare
  Product = Cloudflare Insights
  Lms = Direct
  DataType = "app-activity"
  TimeFormat = "yyyy-MM-dd'T'HH:mm:ssZ"
  Conditions = [ """CEF:""", """destinationServiceName=cloudflare""", """"when":"""" ]
  Fields = [
    """exabeam_host=([^=]+@\s*)?({host}\S+)""",
    """"when":"({time}[^"]+)"""",
    """suser=({user}[^\s]+)""",
    """destinationServicename=({app}[^\s]+)""",
    """flexString1=({activity}[^\s]+)""",
    """src=({src_ip}\d+.\d+.\d+.\d+)""",
    """msg=({additional_info}.+?)\s\w+=""",
  ]
}
```