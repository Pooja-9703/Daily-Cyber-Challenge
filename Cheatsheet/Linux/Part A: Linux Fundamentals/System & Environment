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

> ** Use `hostname` when you only need to quickly identify the system's hostname. Use `hostnamectl` when you need to manage the hostname persistently.

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
id -u username
```
Displays the UID of a specific user.

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
