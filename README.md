# List-RDP-Connections-History
Use powershell to list the RDP Connections History of logged-in users or all users

### List Logged-in Users's RDP Connections History:

Enumerating the registry key values of HKEY_USERS\"+$User.SID+"\Software\Microsoft\Terminal Server Client\Servers\

### List All Users's RDP Connections History:

First use "reg load" to load hive.

Then read the RDP Connections History from HKEY_USERS.

Last you need to use "reg unload" to unload hive. 

[Detals soon]
