Vendor: IBM
===========
### Product: [Lotus Mobile Connect](../ds_ibm_lotus_mobile_connect.md)
### Use-Case: [Lateral Movement](../../../../UseCases/uc_lateral_movement.md)

| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|   2   |   1    |     2      |      3      |    3    |

| Event Type                | Rules                                                                                                                              | Models                              |
| ------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------- |
| authentication-failed     | <b>T1133 - External Remote Services</b><br> ↳ <b>FA-UC-F</b>: Failed activity from a new country                                   |  • <b>UA-UC</b>: Countries for user |
| authentication-successful | <b>T1078 - Valid Accounts</b><b>T1133 - External Remote Services</b><br> ↳ <b>UA-UC-new</b>: Abnormal country for user by new user |  • <b>UA-UC</b>: Countries for user |
| failed-vpn-login          | <b>T1133 - External Remote Services</b><br> ↳ <b>FA-UC-F</b>: Failed activity from a new country                                   |  • <b>UA-UC</b>: Countries for user |
| vpn-login                 | <b>T1078 - Valid Accounts</b><b>T1133 - External Remote Services</b><br> ↳ <b>UA-UC-new</b>: Abnormal country for user by new user |  • <b>UA-UC</b>: Countries for user |