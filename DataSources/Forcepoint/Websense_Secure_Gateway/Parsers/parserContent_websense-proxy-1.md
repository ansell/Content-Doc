#### Parser Content
```Java
{
Name = websense-proxy-1
    Vendor = Forcepoint
    Product = Websense Secure Gateway
    Lms = Direct
    DataType = "web-activity"
    IsHVF = true
    TimeFormat = "yyyy-MM-dd HH:mm:ss"
    Conditions = [ """|Websense|Security|""","""|transaction:""","""srcBytes=""" ]
    Fields = [
      """exabeam_endTime=({time}\d+)""",
      """exabeam_time=({time}\d\d\d\d\-\d\d\-\d\d \d\d:\d\d:\d\d)""",
      """\d{1,2}:\d{1,2}:\d{1,2}\s+({host}[^\s]+)\s*LEEF:""",
      """\sdst=({dest_ip}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})""",
      """\ssrc=({src_ip}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})""",
      """\ssrcPort=({src_port}\d+)""",
      """\sdstPort=({dest_port}\d+)""",
      """\susrName=(-|(?!LDAP:)({user}.+?))\s+\w+=""",
      """\susrName=LDAP:\/\/\S+\s+({user_ou}[^\/]+?)\/({user_fullname}.+?)\s+\w+=""",
      """\|transaction:({action}[^\|]+)""",
      """\smethod=(?:-|({method}[^\s]+))""",
      """\ssrcBytes=({bytes_in}\d+)""",
      """\sdstBytes=({bytes_out}\d+)""",
      """\scontentType=(?:-|({mime}[^=]+)(;.*)?)\s+reason=""",
      """\sproxyStatus-code=({result_code}\d+)""",
      """\scat=({category_id}\d+)""",
      """exabeam_qidName=.+?\s\-\s({category}[^=]+)\s+exabeam_""",
      """\suserAgent=(?:-|({user_agent}.+?))\s+\w+=""",
      """\suserAgent=(?:-|({browser}[\w\-]+))""",
      """\suserAgent=(?:-|({browser}[\w\-]+)\/[\d\._]+)""",
      """\suserAgent=(?:-|({browser}[^\/]+).+({os}iOS|Android|BlackBerry|Windows Phone|BeOS|(?:W|w)indows|(?:L|l)inux|(?:M|m)acintosh|(?:D|d)arwin))""",
      """\suserAgent=(?:-|Mozilla\/.+\(({os}iOS|Android|BlackBerry|Windows Phone|BeOS|(?:X|x)11|(?:W|w)indows|(?:L|l)inux|(?:M|m)acintosh|(?:D|d)arwin).+?({browser}Chrome|Safari|Opera|(?:F|f)irefox|MSIE|Trident))""",
      """\suserAgent=(?:-|Mozilla\/.+\((?:BeOS|(?:X|x)11|(?:W|w)indows|(?:L|l)inux|(?:M|m)acintosh|(?:D|d)arwin).+Gecko\/\d+\s+({browser}\w+))""",
      """\surl=(?:-|({full_url}[^\s"]+))""",
      """\surl=(?:-|({protocol}[^:]+))""",
      """\surl=(?:[^:]+:\/+)({web_domain}[^\/:\s]+)""",
      """\surl=(?:-|\w+:\/+[^\/]+)({uri_path}\/[^?\s]+)""",
      """\surl=(?:-|(?=(?)(?:[^?]+({uri_query}\?[^\s"]+))))""",
      """\surl=(.*?)({top_domain}(?!(?:\d+\.){3}\d+)[^\.\s\/:]+(?=(?:\.(?:com|net|info|edu|org|gov|co|jp|ru|de|ir|it|in|fr|info|pl|nl|es|gr|cz|eu|tv|me|jp|ca|cn|uk|my|cc|id|us|nz|biz|club|io|gg|fi|au|st|tw|asia|sg|ie|li|za))+(\s|\/|$))[^\s\/]+)""",
    ]
  }
```