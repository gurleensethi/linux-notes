# 9. Permissions

- Access can be granted to a group (users are part of groups).

- Permissions can be set for everyone also referred to as `world`.

- Users are assigned a number, can be seen by using commands `id`.

- Users are also primary group ID(gid).

- User accounts are defined in `/etc/passwd`

- For each account `/etc/passwd` file defines id, gid, accounts real name, home directory and login shell.

- Groups are defined in `/etc/group`.

## User permissions

- The first 10 characters of `ls -l some-file.txt` give information regarding its permissions.

- The first character tell the type of file.

- Links always show `rwxrwxrwx`, these are dummy values, the real values existon the actual file.

- The remaining 9 characters represent the permissions as: Owner(3), Group(3),World(3).

- `chmod` is used to change the mode(permissions) of a file or directory. Only the file's owner or superuser can do this.

- Octal number represent each file mode as such.

| Octal | Binary | File Mode |
| :---: | :----: | :-------: |
|   0   |  000   |    ---    |
|   1   |  001   |    --x    |
|   2   |  010   |    -w-    |
|   3   |  011   |    -wx    |
|   4   |  100   |    r--    |
|   5   |  101   |    r-x    |
|   6   |  110   |    rw-    |
|   7   |  111   |    rwx    |

- Example: Change a file's mode -> `chmod 666 some-file.txt`.

- Symbolic Notation for changing modes.

| Symbol |           Meaning           |
| :----: | :-------------------------: |
|   u    | File/Directory owner(user). |
|   g    |        Group owner.         |
|   o    |       Others (World).       |
|   a    |   All (means u, g and o).   |

- Example: `u+x` will add execute permission for user, `u-xw` will remove execute and write permissions for the user. `+x` will add execute permissions for all (ugo). `ugo=wr` Set write and read for everyone, and remove execute if it exists.

- `umsak` is to change the default permission of a created file.

- `su` allows to start a shell as another user.