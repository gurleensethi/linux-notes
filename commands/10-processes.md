# Processes

- On boot kernel launches a program named `init`. This init program further run other shell scripts located in `/etc`.

- Use `ps` to view all processes. `ps aux`.

- `TTY` is teletype, is the controlling terminal for a process. `?` means there is no controlling terminal.

- `STAT` tells the current state of a process.

- `top` command disaplys active (every 3 seconds by default) summary of processes.

- Launch a program without terminal waiting for it by placing a `&` after it. Example: `xlogo &`. The teletype of program will be the terminal it was started from.

- `jobs` command lists all jobs.

- Bring a process to foreground using `fg %1`, where `1` is the job number/jobspec.

- `Ctrl + z` to stop(pause) a program and place it into background.

- Continue execution of a stopped program using `bg %1`.

- Must have permissions to use `kill` with a program.

- Get all list of signals using `kill -l`.