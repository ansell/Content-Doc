#### Parser Content
```Java
{
Name = raw-4663-10
    Vendor = Microsoft
    Product = Microsoft Windows
    Lms = Direct
    DataType = "windows-4663"
    IsHVF = true
    TimeFormat = "yyyy-MM-dd'T'HH:mm:ss"
    Conditions = ["An attempt was made to access an object.", "computer_name"]
    Fields = [
      """({event_name}An attempt was made to access an object)""",
      """"(?:winlog\.)?computer_name\\*":\\*"({host}[^\\"]+)""",
      """@timestamp":"({time}\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d)""",
      """({event_code}4663)""",
      """Object(:|=).*?Object Type(:|=)\s*({file_type}.+?)[\s;]*Object Name(:|=)\s*({file_path}({file_parent}.*?)({file_name}[^\\\/;]+?(\.({file_ext}[^\.;\\]+?))?))[\s;]*Handle ID(:|=)""",
      """Process Name(:|=)\s*(?:|({process}.+?))[\s;]*Access Request Information(:|=)""",
      """Process Name(:|=).*\\({process_name}[^\\;]+?)[\s;]*Access Request Information(:|=)""",
      """Accesses(:|=)\s*({accesses}.+?)[\s;]*Access Mask(:|=)\s*({access_mask}\w+)""",
      """"AccessList\\*":\\*"({accesses}[^"]+?)\s*"""",
      """"Account\\*":\\*"(({domain}[^\\\s"]+)\\+)?({user}[^\\\s"]+)""",
      """"SubjectUserSid\\*":\\*"({user_sid}[^\s"]+)""",
      """"SubjectLogonId\\*":\\*"({logon_id}[^\s"]+)""",
      """"ObjectName\\*":\\*"(-|({file_path}({file_parent}.*?)({file_name}[^\\\/;]+?(\.({file_ext}[^\.;]+?))?)))\s*"""",
      """"ObjectType":"(-|({file_type}[^\s"]+))""",
      """"ProcessName":"(?: |({process}({directory}(?:[^";]+)?[\\\/])?({process_name}[^\\\/";]+?)))\s*"""",
    ]
    DupFields = ["host->dest_host","directory->process_directory"]
  }
```