#### Parser Content
```Java
{
Name = azure-ad-account-password-change
  DataType = "password-change"
  Conditions = [ """Microsoft.aadiam""", """Change user password""", """tenantId":""""]
  Fields = ${MSParserTemplates.azure-ad-activity.Fields} [
    """({event_name}Change user password)""",
    """targetResources":.+?userPrincipalName":"({target_user}[^",]+)""",
    """targetResources":.+?id":"({user_sid}[^",]+)"""
  ]
}
```