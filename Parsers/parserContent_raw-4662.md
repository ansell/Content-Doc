#### Parser Content
```Java
{
Name = raw-4662
  Vendor = Microsoft
  Product = Microsoft Windows
  Lms = Direct
  DataType = "object-access"
  TimeFormat = "MMM dd HH:mm:ss yyyy"
  Conditions = ["""An operation was performed on an object"""]
  Fields = [
    """exabeam_host=([^=]+?@\s*)?({host}[\w.-]+)""",
    """({event_name}An operation was performed on an object)""",
    """({event_code}4662)""",
    """({time}\w+ \d\d \d\d:\d\d:\d\d \d\d\d\d)\s+""",
    """Security ID:\s*(|({user_sid}.+?))\s*Account Name:""",
    """Account Name:\s*(|({user}.+?))\s*Account Domain:""",
    """Account Domain:\s*(|({domain}.+?))\s*Logon ID:""",
    """Object Server:\s*(|({object_class}.+?))\s*Object Type:""",
    """Object Type:\s*(|({activity_type}.+?))\s*Object Name:""",
    """Object Name:\s*(|({object}.+?))\s*Handle ID:""",
    """Logon ID:\s*({logon_id}[^\s]+)\s""",
    """Operation Type:\s*({activity}.+?)\s+Accesses:""",
    """Properties:\s*({properties}.+?)\s+Additional""",
    """Additional Information:\s*({attribute}.+?)\s*(<\/Message>|\s+User:|$)"""
  ]
}
```