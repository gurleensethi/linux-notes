1. Access can be granted to a group (users are part of groups). 
   Permissions can be set for everyone also referred to as 'world'.

2. Users are assigned a number, can be seen by using commands 'id'.
   Users are also primary group ID(gid).
   User accounts are defined in '/etc/passwd'. 
   For each account '/etc/passwd' file defines id, gid, accounts real name, home directory and login shell.
   Groups are defined in '/etc/group'.

3. The first 10 characters of 'ls -l some-file.txt' give information regarding its permissions.
   The first character tell the type of file.
   Links always show 'rwxrwxrwx', these are dummy values, the real values exist on the actual file.
   The remaining 9 characters represent the permissions as: Owner(3), Group(3), World(3).
