Vendor: Juniper VPN
===================
### Product: [Juniper VPN](../ds_juniper_vpn_juniper_vpn.md)
### Use-Case: [Lateral Movement](../../../../UseCases/uc_lateral_movement.md)

| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|   3   |   1    |     2      |      2      |    2    |

| Event Type       | Rules                                                                                                                              | Models                              |
| ---------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------- |
| failed-vpn-login | <b>T1133 - External Remote Services</b><br> ↳ <b>FA-UC-F</b>: Failed activity from a new country                                   |  • <b>UA-UC</b>: Countries for user |
| vpn-login        | <b>T1078 - Valid Accounts</b><b>T1133 - External Remote Services</b><br> ↳ <b>UA-UC-new</b>: Abnormal country for user by new user |  • <b>UA-UC</b>: Countries for user |
| vpn-logout       | <b>T1078 - Valid Accounts</b><br> ↳ <b>DC14g-new</b>: Abnormal number of accessed assets for group of new user                     |                                     |