#### Parser Content
```Java
{
Name = unix-authentication-successful
  Vendor = Unix
  Product = Unix
  Lms = Direct
  DataType = "authentication-successful"
  TimeFormat = "yyyy-MM-dd'T'HH:mm:ss"
  Conditions = [ """successful pam web login:""",""" as """]
  Fields = [
    """\s({time}\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2})\S+\s+({host}[^\s]+)\s+({process_name}[^\s]+)\s+({process_id}\d+)\s""",
    """successful pam web login:\s({user}[^\s@]+)@({src_ip}[\da-fA-F.:]+)""",
    """({outcome}successful) pam web login:"""
  ]
}
```