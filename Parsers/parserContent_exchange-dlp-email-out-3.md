#### Parser Content
```Java
{
Name = exchange-dlp-email-out-3
  Conditions = [ """,MAILBOXRULE,RECEIVE,""", """,Originating,""" ]
  DupFields = [ "recipient->external_address", "external_domain_recipient->external_domain" ]
}
```