#### Parser Content
```Java
{
Name = checkpoint-network-encrypt
  DataType = "network-alert"
  Conditions = [ """CheckPoint""", """product:"""", """action:"accept encrypt"""" ]
  Fields = ${CheckpointParserTemplates.checkpoint-auth.Fields}[
    """event_name:"+({alert_name}[^"]+)""",
    """cu_rule_category:"+({alert_type}[^"]+)""",
    """proto:"+({protocol}[^"]+)""",
    """cu_rule_id:"+({rule_id}[^"]+)""",
    """service:"+({service}\d+)"""
    """cu_action:"+({action}[^"]+)""",
    """cu_detected_by:"+({src_ip}[^"]+)""",
    """ src:"+({src_ip}[A-Fa-f:\d.]+)""",
    """dst:"+({dest_ip}[^"]+)""",
   
   ]
}
```