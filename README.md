# Description

CLI interface for listing/downloading/managing Proton-GE compat tool installations

# Usage

1. Set the env var `PGE_COMPAT_DIR` before using the script.
The default path is `<Steam path>/compatibilitytools.d`.
On most environments, this defaults to: `$HOME/.local/share/Steam/compatibilitytools.d`

2. Invoke `pge` with one of the following arguments:

- info: print version info
- list: list installed Proton-GE versions
- update: download and unpack latest Proton-GE
- jump: jump to compat tools dir
- news: get latest release notes
- notify: print if upstream PGE has updates (for use in cronjobs/monitors)
    Silently returns 0 if up to date
    Returns 1 and version number if upstream is newer
- remove: list versions and remove version at the numbered index

3. Invoke `pge` with no arguments to print the usage instructions and the above list of commands.
