#### Parser Content
```Java
{
Name = cef-mimecast-dlp-email
  Vendor = Mimecast
  Product = Mimecast
  Lms = ArcSight
  DataType = "dlp-email-alert"
  TimeFormat = "yyyy-MM-dd'T'HH:mm:ss.SSSZ"
  Conditions = [ """CEF:""", """|SkyFormation Cloud Apps Security|""", """destinationServiceName=Mimecast Email Security""", """"Dir":"""", """"Sender":"""", """"Rcpt":"""" ]
  Fields = [
    """"acc":"({host}[^",]+)"""",
    """({time}\d+-\d+-\d+T\d+:\d+:\d+\.\d+Z)\s+[\w\-.]+\s+Skyformation""",
    """request=({outcome}[^=]+?)\s+(\w+=|$)""",
    """suser=(<>|(({user_email}[^\s@]+@[^\s@]+)|({user}[^\s]+)))""",
    """"Rcpt":"({recipients}({recipient}[^\s@;,"]+@[^\s@;,"]+)[^"]*)"""",
    """"Subject":"(|({subject}[^"]+))""""
    """requestMethod=({direction}[^=]*?)\s+(\w+=|$)""",
    """"Dir":"({direction}[^"]+?)""""
    """src=({src_ip}[A-Fa-f:\d.]+)""",
    """"aCode":"(|({alert_id}[^"]+?))"""",
    """"Rcpt":"({external_address}[^\s@;,]+@({external_domain}[^\s@;,"]+))""",
    """Dir=Inbound[^\}]+?"Sender":"(<>|({external_address}[^\s@;,]+@({external_domain}[^\s@;,"]+)))"""", 
    """"Sender":"(<>|({sender}[^"]+))""""
  ]
}
```