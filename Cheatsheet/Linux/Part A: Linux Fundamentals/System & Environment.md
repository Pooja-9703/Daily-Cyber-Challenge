# System & Environment

## 1. `uname`

**Use:** Displays information about the Linux system and kernel.

### Syntax

```bash
uname [OPTION]
```

### Common Options

| Option | Description |
|---|---|
| `-a` | Displays all available system information. |
| `-s` | Displays the kernel name. |
| `-n` | Displays the system's network hostname. |
| `-r` | Displays the kernel release/version. |
| `-v` | Displays the kernel version/build information. |
| `-m` | Displays the machine hardware architecture. |
| `-p` | Displays the processor type, if available. |
| `-i` | Displays the hardware platform, if available. |
| `-o` | Displays the operating system. |

---

## 2. `hostname`

**Use:** Displays the system hostname. It can also be used to temporarily change the hostname.

### Syntax

```bash
hostname [OPTION]
hostname [OPTION] [NAME]
```

### Common Options

| Option | Description |
|---|---|
| `-s` | Displays only the short hostname. |
| `-f` | Displays the Fully Qualified Domain Name (FQDN). |
| `-d` | Displays the DNS domain name. |
| `-i` | Displays the IP address associated with the hostname. |
| `-I` | Displays all configured IP addresses. |
| `-a` | Displays hostname aliases, if available. |

### Changing the Hostname

```bash
sudo hostname new-hostname
```

Temporarily changes the hostname for the current system session. Use `hostnamectl` for a persistent hostname change on systems using `systemd`.

> Use `hostname` when you only need to quickly identify the system's hostname. Use `hostnamectl` when you need to manage the hostname persistently.

---

## 3. `hostnamectl`

**Use:** Displays and manages the system hostname and related system information on systems using `systemd`.

### Syntax

```bash
hostnamectl [OPTIONS] [COMMAND]
```

### Common Commands (Subcommands)

| Command | Description |
|---|---|
| `status` | Displays the hostname and system information. |
| `hostname` | Displays the current hostname. |
| `set-hostname NAME` | Sets the system hostname. |

### `set-hostname` Options

| Option | Description |
|---|---|
| `--static` | Sets the static hostname. |
| `--pretty` | Sets the pretty hostname. |
| `--transient` | Sets the transient hostname. |

### Other Common Options

| Option | Description |
|---|---|
| `-H, --host=HOST` | Operates on a remote host. |
| `-M, --machine=CONTAINER` | Operates on a local container. |
| `--no-ask-password` | Does not prompt for authentication when possible. |

### Examples

```bash
hostnamectl
```
Displays hostname and system information.

```bash
hostnamectl status
```
Displays the current hostname along with operating system, kernel, architecture, and related information.

```bash
hostnamectl hostname
```
Displays the current hostname.

```bash
sudo hostnamectl set-hostname server01
```
Sets the system hostname persistently.

### Setting Different Hostname Types

```bash
sudo hostnamectl set-hostname server01 --static
```
Sets the static hostname.

```bash
sudo hostnamectl set-hostname "Production Server" --pretty
```
Sets the human-readable pretty hostname.

```bash
sudo hostnamectl set-hostname server01 --transient
```
Sets the transient hostname.

---

## 4. `uptime`

**Use:** Displays how long the system has been running, the number of logged-in users, and system load averages.

### Syntax

```bash
uptime [OPTION]
```

### Common Options

| Option | Description |
|---|---|
| `-p` | Displays uptime in a human-readable format. |
| `-s` | Displays the date and time when the system was started. |
| `--pretty` | Same as `-p`. |
| `--since` | Same as `-s`. |

---

## 5. `whoami`

**Use:** Displays the username of the currently logged-in user.

### Syntax

```bash
whoami
```

### Options

`whoami` normally does not require options for everyday use.

---

## 6. `id`

**Use:** Displays the user ID (UID), group ID (GID), and group memberships of a user.

### Syntax

```bash
id [OPTION] [USERNAME]
```

### Common Options

| Option | Description |
|---|---|
| `-u` | Displays the user ID (UID). |
| `-g` | Displays the effective group ID (GID). |
| `-G` | Displays all group IDs the user belongs to. |
| `-n` | Displays names instead of numeric IDs. |
| `-r` | Displays the real ID instead of the effective ID. |
| `-a` | Displays all available identity information. |

### Useful Combinations

```bash
id -un
```
Displays the current username.

```bash
id -Gn
```
Displays all groups the current user belongs to by name.

```bash
id -Gn username
```
Displays the groups associated with a specific user.

---

## 7. `who`

**Use:** Displays information about users currently logged into the system.

### Syntax

```bash
who [OPTION]
```

### Common Options

| Option | Description |
|---|---|
| `-a` | Displays all available information. |
| `-b` | Displays the time of the last system boot. |
| `-H` | Displays column headings. |
| `-q` | Displays logged-in usernames and the number of users. |
| `-r` | Displays the current runlevel. |
| `-T` | Displays the user's terminal status. |
| `-u` | Displays additional information about logged-in users. |

---
## 8. `w`

**Use:** Displays information about currently logged-in users and their activity.

### Syntax

```bash
w [OPTIONS] [USER]
```

### Common Options

| Option | Description |
|---|---|
| `-h` | Omits the header. |
| `-u` | Ignores the username column when calculating current processes. |
| `-s` | Uses the short format; omits login time, JCPU, and PCPU. |
| `-f` | Toggles the display of the `FROM` field. |
| `-i` | Displays the IP address instead of the hostname in the `FROM` field. |

### Examples

```bash
w username
```
Displays information for a specific user.

---

## 9. `last`

**Use:** Displays recent login history from the system's login records.

### Syntax

```bash
last [OPTIONS] [USERNAME] [TTY]
```

### Common Options

| Option | Description |
|---|---|
| `-n NUM` | Displays only the specified number of entries. |
| `-a` | Displays the hostname in the last column. |
| `-i` | Displays IP addresses instead of hostnames. |
| `-x` | Includes system shutdowns, runlevel changes, and other system events. |
| `-F` | Displays full login and logout times and dates. |
| `-R` | Hides the hostname field. |

### Examples

```bash
last username
```
Displays login history for a specific user.

---

## 10. `lastlog`

**Use:** Displays the most recent login for each user account.

### Syntax

```bash
lastlog [OPTIONS]
```

### Common Options

| Option | Description |
|---|---|
| `-u USER` | Displays the last login information for a specific user. |
| `-b DAYS` | Displays users whose last login was older than the specified number of days. |
| `-t DAYS` | Displays users whose last login was more recent than the specified number of days. |
| `-C` | Displays the time in a more compact format. |

### Examples

```bash
lastlog -u username
```
Displays the most recent login for a specific user.

```bash
lastlog -b 30
```
Displays users whose last login was more than 30 days ago.

---

## 11. `date`

**Use:** Displays or sets the system date and time.

### Syntax

```bash
date [OPTIONS] [+FORMAT]
date [OPTIONS] [MMDDhhmm[[CC]YY][.ss]]
```

### Common Options

| Option | Description |
|---|---|
| `-u` | Displays or sets the time in UTC. |
| `-d STRING` | Displays the date/time described by the given string. |
| `-R` | Displays the date and time in RFC 5322 format. |
| `-I` | Displays the date in ISO 8601 format. |
| `-s STRING` | Sets the system date/time. Requires appropriate privileges. |

### Common Format Specifiers

| Format | Description |
|---|---|
| `%Y` | Four-digit year. |
| `%m` | Month (`01–12`). |
| `%d` | Day of the month. |
| `%H` | Hour (`00–23`). |
| `%M` | Minute. |
| `%S` | Second. |
| `%T` | Time in `HH:MM:SS` format. |
| `%F` | Date in `YYYY-MM-DD` format. |
| `%A` | Full weekday name. |
| `%B` | Full month name. |

### Examples

```bash
date '+%Y-%m-%d'
```
Displays the date as `YYYY-MM-DD`.

```bash
date '+%Y-%m-%d %H:%M:%S'
```
Displays the date and time in a standard format.

```bash
date -d "tomorrow"
```
Displays tomorrow's date.

---

## 12. `timedatectl`

**Use:** Queries and controls the system clock, time zone, and time synchronization settings.

### Syntax

```bash
timedatectl [OPTIONS] [COMMAND]
```

### Common Commands (Subcommands)

| Command | Description |
|---|---|
| `status` | Displays current time, time zone, NTP status, and clock settings. |
| `show` | Displays the time and related settings in machine-readable form. |
| `list-timezones` | Lists available time zones. |
| `set-time TIME` | Sets the system time. |
| `set-timezone ZONE` | Sets the system time zone. |
| `set-ntp BOOL` | Enables or disables network time synchronization. |
| `timesync-status` | Displays the status of systemd time synchronization. |

### Common Options

| Option | Description |
|---|---|
| `-a, --all` | Displays all available properties with `show`. |
| `-p, --property=NAME` | Limits output to a specific property. |
| `--value` | Prints only property values. |
| `-H, --host=HOST` | Operates on a remote host. |

### Examples

```bash
timedatectl list-timezones | grep Asia/Kolkata
```
Searches for the India time zone.

```bash
sudo timedatectl set-timezone Asia/Kolkata
```
Sets the system time zone to India Standard Time.

```bash
timedatectl timesync-status
```
Displays time synchronization status.

---

## 13. `cal`

**Use:** Displays the current month's calendar.

### Syntax

```bash
cal [OPTIONS] [[MONTH] YEAR]
```

### Common Options

| Option | Description |
|---|---|
| `-1` | Displays a single month. |
| `-3` | Displays the previous, current, and next month. |
| `-y` | Displays the calendar for the entire current year. |
| `-m` | Displays Monday as the first day of the week. |
| `-j` | Displays Julian day numbers instead of day-of-month numbers. |

### Examples

```bash
cal 12 2026
```
Displays December 2026.

---

## 14. `arch`

**Use:** Displays the system's machine architecture.

### Syntax

```bash
arch
```

### Options

`arch` does not normally require options for basic use.

### Examples

```bash
arch
```

---

## 15. `env`

**Use:** Displays environment variables or runs a command with a modified environment.

### Syntax

```bash
env [OPTION]... [-] [NAME=VALUE]... [COMMAND [ARG]...]
```

### Common Options

| Option | Description |
|---|---|
| `-i` | Starts with an empty environment. |
| `-0` | Ends each output entry with a null character instead of a newline. |
| `-u NAME` | Removes the specified variable from the environment. |
| `-C DIR` | Changes to the specified directory before running the command. |
| `--ignore-environment` | Same as `-i`. |

### Examples

```bash
env | grep PATH
```
Displays environment variables related to `PATH`.

```bash
env VAR=value command
```
Runs a command with an additional environment variable.

```bash
env -u VARIABLE command
```
Runs a command after removing the specified environment variable.

```bash
env -i command
```
Runs a command with an empty environment.

---

## 16. `printenv`

**Use:** Displays all environment variables.

### Syntax

```bash
printenv [OPTION] [VARIABLE]
```

### Common Options

| Option | Description |
|---|---|
| `-0` | Ends each output entry with a null character instead of a newline. |

### Examples

```bash
printenv PATH
```
Displays the value of the `PATH` variable.

```bash
printenv HOME
```
Displays the user's home directory.

```bash
printenv SHELL
```
Displays the user's default shell.

---

## 17. `set`

**Use:** Displays shell variables, functions, and environment information, and can also modify shell options.

### Syntax

```bash
set [OPTION]
set [OPTION] [ARGUMENT]
```

### Common Options

| Option | Description |
|---|---|
| `-a` | Automatically exports variables assigned or modified afterward. |
| `-e` | Exits the shell when a command returns a non-zero status, with defined exceptions. |
| `-u` | Treats unset variables as an error when expanded, with defined exceptions. |
| `-x` | Prints commands and their arguments before executing them. |
| `-n` | Reads commands without executing them. |
| `-f` | Disables pathname expansion (globbing). |
| `-o OPTION` | Enables or disables a specific shell option. |

### Examples

```bash
set -x
```
Displays commands before they are executed, useful for debugging shell scripts.

```bash
set +x
```
Disables command tracing.

---

## 18. `echo`

**Use:** Displays text or the value of variables to standard output.

### Syntax

```bash
echo [OPTION]... [STRING]...
```

### Common Options

| Option | Description |
|---|---|
| `-n` | Does not print the trailing newline. |
| `-e` | Enables interpretation of backslash escape sequences. |
| `-E` | Disables interpretation of escape sequences; this is the default in many implementations. |

### Examples

```bash
echo "Hello World"
```
Displays text.

```bash
echo $HOME
```
Displays the value of the `HOME` variable.

```bash
echo -n "Hello"
```
Prints text without a trailing newline.

```bash
echo -e "Hello\nWorld"
```
Interprets `\n` as a newline.

---

## 19. `printf`

**Use:** Formats and prints text to standard output. It provides more predictable formatting than `echo` and is commonly used in shell scripts.

### Syntax

```bash
printf FORMAT [ARGUMENT]...
```

### Common Format Specifiers

| Format | Description |
|---|---|
| `%s` | String. |
| `%d` | Decimal integer. |
| `%f` | Floating-point number. |
| `%x` | Hexadecimal integer. |
| `%o` | Octal integer. |
| `%%` | Prints a literal `%` character. |
| `\n` | Newline. |
| `\t` | Tab. |

### Examples

```bash
printf "Name: %s\n" "Pooja"
```
Prints a formatted string.

```bash
printf "Number: %d\n" 10
```
Prints a formatted integer.

```bash
printf "%s\t%s\n" "Name" "Age"
```
Prints values separated by a tab.

---

## 20. `clear`

**Use:** Clears the visible contents of the terminal screen.

### Syntax

```bash
clear [OPTION]
```

### Common Options

| Option | Description |
|---|---|
| `-T TERM` | Uses the specified terminal type. |
| `-V` | Displays version information. |

### Examples

```bash
Ctrl + L
```
Common keyboard shortcut that also clears the visible terminal screen in many shells.

---

## 21. `history`

**Use:** Displays previously executed commands from the shell history (command history).

### Syntax

```bash
history [N]
history [OPTIONS]
```

### Common Options

| Option | Description |
|---|---|
| `-c` | Clears the current shell history. |
| `-d OFFSET` | Deletes the history entry at the specified offset. |
| `-w` | Writes the current history to the history file. |
| `-r` | Reads the history file and adds its contents to the current history. |
| `-a` | Appends new history entries to the history file. |
| `-n` | Reads new history entries from the history file. |

### Examples

```bash
history 10
```
Displays the last 10 commands.

```bash
history | grep ssh
```
Searches command history for commands containing `ssh`.

```bash
history | grep sudo
```
Searches command history for commands containing `sudo`.

```bash
history -c
```
Clears the current shell history.

---
