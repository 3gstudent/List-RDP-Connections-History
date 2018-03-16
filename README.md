# List-RDP-Connections-History
Use powershell to list the RDP Connections History of logged-in users or all users

### List Logged-in Users' RDP Connections History

Enumerating the registry key values of HKEY_USERS\"+$User.SID+"\Software\Microsoft\Terminal Server Client\Servers\

### List All Users' RDP Connections History

Realization ideas:

- First use "reg load" to load hive.
- Then read the RDP Connections History from HKEY_USERS.
- Last you need to use "reg unload" to unload hive. 

**Note:**

The script automatically implements the above operation,there is no need for a GUI. :)


More Details:

[渗透技巧——获得Windows系统的远程桌面连接历史记录](https://3gstudent.github.io/3gstudent.github.io/%E6%B8%97%E9%80%8F%E6%8A%80%E5%B7%A7-%E8%8E%B7%E5%BE%97Windows%E7%B3%BB%E7%BB%9F%E7%9A%84%E8%BF%9C%E7%A8%8B%E6%A1%8C%E9%9D%A2%E8%BF%9E%E6%8E%A5%E5%8E%86%E5%8F%B2%E8%AE%B0%E5%BD%95/)
