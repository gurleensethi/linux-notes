# The Environment

- `printenv` only displays environment variables.

- `set` displays both environment and shell variables.

- Two types of shells: `Login Shell` and `Non-Login Shell`. Different environment files are read, based on the shell being started.

- `PATH=$PATH:$HOME/bin` translates to `PATH = [existing value of PATH]:[path to home]/bin`. This creates a ":"(colon) separated list of paths that the shell uses to search for commands.