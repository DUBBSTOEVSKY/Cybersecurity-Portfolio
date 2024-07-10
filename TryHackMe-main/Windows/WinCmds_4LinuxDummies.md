# Windows Command Line Cheat Sheet with Linux Cross-References

## Basic Navigation
- **`dir` (Windows)**: Peek inside your folder.
  - *Example*: `dir` lists all files and folders in your current directory.
  - **Linux Equivalent**: `ls`
    - *Example*: `ls` lists files and folders in your current directory.
    - *Difference*: `ls` has more options for formatting and sorting the output.

- **`cd` (Windows)**: Teleport to a different folder.
  - *Example*: `cd Documents` moves you to the Documents folder.
  - **Linux Equivalent**: `cd`
    - *Example*: `cd Documents` works the same way in Linux.
    - *Difference*: No significant difference.

- **`mkdir` (Windows)**: Create a new folder.
  - *Example*: `mkdir NewFolder` creates a new folder named "NewFolder".
  - **Linux Equivalent**: `mkdir`
    - *Example*: `mkdir NewFolder` works the same way in Linux.
    - *Difference*: No significant difference.

## File Operations
- **`copy` (Windows)**: Duplicate files.
  - *Example*: `copy file.txt backup.txt` copies `file.txt` to `backup.txt`.
  - **Linux Equivalent**: `cp`
    - *Example*: `cp file.txt backup.txt` duplicates `file.txt` in Linux.
    - *Difference*: `cp` offers additional options like `-r` for recursive copying.

- **`move` (Windows)**: Relocate files.
  - *Example*: `move file.txt D:\Backup` moves `file.txt` to the D:\Backup folder.
  - **Linux Equivalent**: `mv`
    - *Example*: `mv file.txt /backup` moves `file.txt` in Linux.
    - *Difference*: Syntax and usage are similar, but `mv` in Linux is often used for renaming files too.

- **`del` (Windows)**: Delete files.
  - *Example*: `del file.txt` deletes `file.txt`.
  - **Linux Equivalent**: `rm`
    - *Example*: `rm file.txt` removes `file.txt` in Linux.
    - *Difference*: `rm` has options like `-r` for directories and `-f` for force deletion.

- **`ren` (Windows)**: Rename files.
  - *Example*: `ren oldname.txt newname.txt` changes the name of `oldname.txt` to `newname.txt`.
  - **Linux Equivalent**: `mv`
    - *Example*: `mv oldname.txt newname.txt` renames the file in Linux.
    - *Difference*: `mv` in Linux serves dual purposes for moving and renaming files.

## System Information
- **`systeminfo` (Windows)**: Get the scoop on your PC.
  - *Example*: `systeminfo` shows detailed info about your computer’s hardware and software.
  - **Linux Equivalent**: `uname -a` and `lshw`
    - *Example*: `uname -a` for kernel info, `lshw` for hardware details.
    - *Difference*: Linux uses multiple commands for different types of system information.

- **`msinfo32` (Windows)**: Open System Information tool.
  - *Example*: `msinfo32` launches a window with a comprehensive overview of your system.
  - **Linux Equivalent**: `hardinfo`
    - *Example*: `hardinfo` opens a graphical system information tool.
    - *Difference*: `hardinfo` needs to be installed and is more detailed.

- **`resmon` (Windows)**: Monitor your resources.
  - *Example*: `resmon` opens Resource Monitor to see how your computer’s resources are being used.
  - **Linux Equivalent**: `htop` or `top`
    - *Example*: `htop` provides an interactive process viewer, `top` shows real-time system info.
    - *Difference*: `htop` is more interactive, `top` is available by default.

## Networking
- **`ipconfig` (Windows)**: Check your network settings.
  - *Example*: `ipconfig` displays your IP address and other network details.
  - **Linux Equivalent**: `ifconfig` or `ip`
    - *Example*: `ifconfig` for network interfaces, `ip a` for IP addresses.
    - *Difference*: `ip` is more modern and preferred in Linux.

- **`ping` (Windows)**: Test network connectivity.
  - *Example*: `ping google.com` checks if you can reach Google.
  - **Linux Equivalent**: `ping`
    - *Example*: `ping google.com` works the same way in Linux.
    - *Difference*: No significant difference.

- **`netstat` (Windows)**: View active connections.
  - *Example*: `netstat` shows all current network connections and listening ports.
  - **Linux Equivalent**: `netstat`
    - *Example*: `netstat` functions similarly in Linux.
    - *Difference*: `ss` is often used in Linux for more detailed socket statistics.

- **`tracert` (Windows)**: Trace the route packets take.
  - *Example*: `tracert google.com` shows the path your data takes to reach Google.
  - **Linux Equivalent**: `traceroute`
    - *Example*: `traceroute google.com` works the same way in Linux.
    - *Difference*: Name and some options differ.

## Task Management
- **`tasklist` (Windows)**: See what’s running.
  - *Example*: `tasklist` displays all running processes.
  - **Linux Equivalent**: `ps`
    - *Example*: `ps aux` lists running processes in Linux.
    - *Difference*: `ps` has different options and output formatting.

- **`taskkill` (Windows)**: Terminate processes.
  - *Example*: `taskkill /IM notepad.exe` closes Notepad.
  - **Linux Equivalent**: `kill` or `pkill`
    - *Example*: `kill [PID]` or `pkill notepad` terminates processes.
    - *Difference*: `kill` needs process IDs, `pkill` can use process names.

- **`shutdown` (Windows)**: Power down your PC.
  - *Example*: `shutdown /s /t 0` shuts down your computer immediately.
  - **Linux Equivalent**: `shutdown`
    - *Example*: `shutdown now` or `shutdown -h now` for immediate shutdown.
    - *Difference*: Options are slightly different.

## File System Utilities
- **`chkdsk` (Windows)**: Check and repair disk issues.
  - *Example*: `chkdsk C: /f` checks and fixes errors on the C: drive.
  - **Linux Equivalent**: `fsck`
    - *Example*: `fsck /dev/sda1` checks and repairs filesystem issues.
    - *Difference*: `fsck` is used with device names.

- **`sfc /scannow` (Windows)**: Scan and repair system files.
  - *Example*: `sfc /scannow` scans your system for corrupted files and repairs them.
  - **Linux Equivalent**: `apt-get check` or `dpkg --audit`
    - *Example*: `dpkg --audit` checks for broken packages.
    - *Difference*: Linux commands focus on package integrity.

- **`attrib` (Windows)**: Change file attributes.
  - *Example*: `attrib +r file.txt` makes `file.txt` read-only.
  - **Linux Equivalent**: `chmod`
    - *Example*: `chmod 444 file.txt` makes `file.txt` read-only.
    - *Difference*: `chmod` uses numeric codes for permissions.

## Advanced Tools
- **`gpedit.msc` (Windows)**: Open Group Policy Editor.
  - *Example*: `gpedit.msc` launches the Group Policy Editor.
  - **Linux Equivalent**: No direct equivalent, uses `nano` or `vi` to edit config files.
    - *Example*: Edit `/etc` files for policy changes.

- **`regedit` (Windows)**: Open Registry Editor.
  - *Example*: `regedit` opens the Registry Editor.
  - **Linux Equivalent**: No direct equivalent, uses text editors for config files.
    - *Example*: Edit config files in `/etc` with `nano` or `vi`.

- **`services.msc` (Windows)**: Manage background services.
  - *Example*: `services.msc` opens the Services window.
  - **Linux Equivalent**: `systemctl`
    - *Example*: `systemctl status` to view services, `systemctl start [service]` to start a service.
    - *Difference*: `systemctl` is command-line based.

- **`eventvwr` (Windows)**: View system logs.
  - *Example*: `eventvwr` opens Event Viewer to see logs of system events.
  - **Linux Equivalent**: `journalctl`
    - *Example*: `journalctl` shows system logs.
    - *Difference*: `journalctl` is command-line based and requires options for detailed views.

## Note

These are just a few of the commands I've learned, but cross-referenced to help out my Linux peeps out there! I hope they help. 