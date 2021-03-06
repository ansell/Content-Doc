#### Parser Content
```Java
{
Name = skyformation-cloudflare-waf-1
  Vendor = Cloudflare
  Product = Cloudflare WAF
  Lms = Direct
  DataType = "web-activity"
  IsHVF = true
  TimeFormat = "yyyy-MM-dd'T'HH:mm:ss.SSSZ"
  Conditions = [ """|Skyformation|""", """destinationServiceName=Cloudflare""", """"ClientIP":"""", """"FirewallMatchesActions":""" ]
  Fields = [
    """({time}\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d.\d\d\dZ)\s+[^\s]+\s+Skyformation""",
    """"ClientRequestHost":"({host}[^"]+)""",
    """"RayID":"({alert_id}[^"]+)""",
    """"WAFAction":"(unknown|({proxy_action}[^"]+))""",
    """"WAFRuleID":"({event_code}[^"]+)""",
    """"WAFRuleMessage":"({additional_info}[^"]+)""",
    """dhost=({dest_host}[^\s]+)""",
    """suser=(anonymous|({user}[^\s]+))""",
    """"ClientDeviceType":"({device_type}[^"]+)""",
    """"ClientCountry":"({src_country}[^"]+)""",
    """"ClientIP":"(?:["]+|({src_ip}[A-Fa-f:\d.]+))""",
    """"ClientSrcPort":({src_port}\d+)""",
    """"ClientRequestUserAgent":"({user_agent}[^"]+)""",
    """"ClientRequestBytes":({bytes_in}\d+)""",
    """"EdgeResponseBytes":({bytes_out}\d+)""",
    """"EdgeResponseStatus":({result_code}({edge_response_status}\d\d\d))"""
    """"OriginResponseStatus":({result_code}({origin_response_status}\d\d\d))"""
    """"EdgeServerIP":"({dest_ip}[A-Fa-f:\d.]+)""",
    """"OriginIP":"({dest_ip}[A-Fa-f:\d.]+)"*[^=]+?OriginResponseBytes":({bytes_out}\d+)""",
    """"OriginIP":"(?:["]+|({dest_ip}[A-Fa-f:\d.]+))""",
    """"ClientRequestMethod":"(UNKNOWN|({method}[^"]+))""",
    """"FirewallMatchesActions[":\[]+(?:["\]]+|({action}[^,"]+))""",
    """\|act=({action}[^\s]+)\s\w+=""",
    """"ClientRequestHost":"({web_domain}[^"]+)""",
    """"clientRequestHTTPHost"+:"+[^\s"?=]*?({top_domain}(?!(?:\d+\.){3}\d+)[^\.\s]+(?=(?:\.(?:com|net|info|edu|org|gov|co|jp|ru|de|ir|it|in|fr|info|pl|nl|es|gr|cz|eu|tv|me|jp|ca|cn|uk|my|cc|id|us|nz|biz|club|io|gg|fi|au|st|tw|asia|sg|ie|li|za)(?::\d+)?)+(?:\s\w+=|\/|))[^"\s:\/]+)""",
    """"ClientRequestURI":"({uri_path}[^"\?\s]+)(?:\?({uri_query}[^?\s"]+))?""",
    """"ClientRequestProtocol":"({protocol}[^"]+)""",
    """"SecurityLevel":"({alert_severity}[^"]+)""",
    """"ClientRequestReferer":"({referrer}[^"]+?)",""",
    """"ClientRequestUserAgent[":]+[^=]+?({os}iOS|Android|BlackBerry|Windows Phone|BeOS|(?:X|x)11|(?:W|w)indows|(?:L|l)inux|(?:M|m)acintosh|(?:D|d)arwin)([^=]+?({browser}Chrome|Safari|Opera|(?:F|f)irefox|MSIE|Trident))?"""
    ]
}
```