#### Parser Content
```Java
{
Name = raw-5145
    Vendor = Microsoft
    Product = Microsoft Windows
    Lms = Direct
    DataType = "share-access"
    TimeFormat = "yyyy-MM-dd HH:mm:ss"
    Conditions = ["""A network share object was checked to see whether client can be granted desired access""", """Account Name:"""]
    Fields = [
      """({event_name}A network share object was checked to see whether client can be granted desired access)""",
      """({event_code}5145)""",
      """exabeam_host=({host}[^\s]+)""",
      """exabeam_time=({time}\d\d\d\d-\d\d-\d\d \d\d:\d\d:\d\d)"""
      """({host}[\w\-.]+)\s+(?i)((audit|success)( |_)(success|audit))""",
      """Logon ID:\s*((\\)[rnt])*({logon_id}\S+?)((\\)[rnt])*\s*Network Information:""",
      """Account Name:\s*((\\)[rnt])*({user}\S+?)((\\)[rnt])*\s*Account Domain:""",
      """Account Domain:\s*((\\)[rnt])*({domain}\S+?)((\\)[rnt])*\s*Logon ID:""",
      """Object Type:\s*((\\)[rnt])*({file_type}[^:]+?)((\\)[rnt])*\s*Source Address:""",
      """Source Address:\s*((\\)[rnt])*(::1|({src_ip}[A-Fa-f:\d.]+?))((\\)[rnt])*\s*Source Port:""",
      """Share Name:\s*((\\)[rnt])*(?:\\\\\*\\)?({share_name}[^=]+?)((\\)[rnt])*\s*Share Path:""",
      """Share Path:\s*((\\)[rnt])*(?:[\\\?]+)?(?:\s*|({share_path}(({d_parent}[^=]+?)\\)?(|({d_name}[^\\]*?)))\\?)((\\)[rnt])*\s*Relative Target Name:""",
      """Relative Target Name:\s*((\\)[rnt])*\\?(?:\s*|(?:({f_parent}[^=]+?)\\)?(|({file_name}[^\\:\/]+?(?:\.({file_ext}[^\.]+?))?))(?:\\HEAD|:[^=]+?|\\|\s|((\\)[rnt])*)\s*)Access Request Information:""",
      """Accesses:[^=]*({accesses}SYNCHRONIZE|Execute|Traverse|Read|READ|WRITE_DAC|WRITE_OWNER|WriteAttributes|WriteEA|WriteData|AppendData|delete|Delete)[^=]*Access Check Results:""",
      """Access Check Results:\s*({outcome}-)\s""",
      """Access Check Results:[^=]*({outcome}Granted|Denied)\s+by""",
    ]
    DupFields = ["host->dest_host"]
  }
```