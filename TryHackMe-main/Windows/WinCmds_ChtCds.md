# Windows Command Line Cheat Sheet (Cheat Codes)

## Basic Navigation
- **`dir`**: Peek inside your folder.
  - *Example*: `dir` lists all files and folders in your current directory. Think of it as opening a drawer to see what’s inside.

- **`cd`**: Teleport to a different folder.
  - *Example*: `cd Documents` moves you to the Documents folder. Use `cd ..` to go back up a level.

- **`mkdir`**: Create a new folder.
  - *Example*: `mkdir NewFolder` creates a new folder named "NewFolder". Perfect for organizing your files.

## File Operations
- **`copy`**: Duplicate files.
  - *Example*: `copy file.txt backup.txt` copies `file.txt` to `backup.txt`. Handy for making backups.

- **`move`**: Relocate files.
  - *Example*: `move file.txt D:\Backup` moves `file.txt` to the D:\Backup folder. Great for tidying up.

- **`del`**: Delete files.
  - *Example*: `del file.txt` deletes `file.txt`. Use with caution, as it’s permanent!

- **`ren`**: Rename files.
  - *Example*: `ren oldname.txt newname.txt` changes the name of `oldname.txt` to `newname.txt`.

## System Information
- **`systeminfo`**: Get the scoop on your PC.
  - *Example*: `systeminfo` shows detailed info about your computer’s hardware and software. It’s like reading your PC’s resume.

- **`msinfo32`**: Open System Information tool.
  - *Example*: `msinfo32` launches a window with a comprehensive overview of your system.

- **`resmon`**: Monitor your resources.
  - *Example*: `resmon` opens Resource Monitor to see how your computer’s resources are being used.

## Networking
- **`ipconfig`**: Check your network settings.
  - *Example*: `ipconfig` displays your IP address and other network details. Use `ipconfig /all` for more info.

- **`ping`**: Test network connectivity.
  - *Example*: `ping google.com` checks if you can reach Google. Useful for troubleshooting internet issues.

- **`netstat`**: View active connections.
  - *Example*: `netstat` shows all current network connections and listening ports. Good for network diagnostics.

- **`tracert`**: Trace the route packets take.
  - *Example*: `tracert google.com` shows the path your data takes to reach Google. Useful for identifying network delays.

## Task Management
- **`tasklist`**: See what’s running.
  - *Example*: `tasklist` displays all running processes. It’s like opening Task Manager in list form.

- **`taskkill`**: Terminate processes.
  - *Example*: `taskkill /IM notepad.exe` closes Notepad. Add `/F` to force close.

- **`shutdown`**: Power down your PC.
  - *Example*: `shutdown /s /t 0` shuts down your computer immediately. Replace `/s` with `/r` to restart.

## File System Utilities
- **`chkdsk`**: Check and repair disk issues.
  - *Example*: `chkdsk C: /f` checks and fixes errors on the C: drive.

- **`sfc /scannow`**: Scan and repair system files.
  - *Example*: `sfc /scannow` scans your system for corrupted files and repairs them.

- **`attrib`**: Change file attributes.
  - *Example*: `attrib +r file.txt` makes `file.txt` read-only. Use `-r` to remove read-only attribute.

## Advanced Tools
- **`gpedit.msc`**: Open Group Policy Editor.
  - *Example*: `gpedit.msc` launches the Group Policy Editor, where you can change local policy settings.

- **`regedit`**: Open Registry Editor.
  - *Example*: `regedit` opens the Registry Editor, allowing you to view and edit the Windows registry.

- **`services.msc`**: Manage background services.
  - *Example*: `services.msc` opens the Services window where you can start, stop, and manage services.

- **`eventvwr`**: View system logs.
  - *Example*: `eventvwr` opens Event Viewer to see logs of system events, useful for troubleshooting errors.

## Fun and Practical Uses
- **Setting Up a File Structure**:
  - Use `mkdir` to create folders for projects, `cd` to navigate, and `copy` to duplicate essential files.

- **Troubleshooting Network Issues**:
  - Use `ping` to check connectivity, `tracert` to identify slow hops, and `netstat` to see active connections.

- **Managing System Performance**:
  - Use `tasklist` to see what’s running, `taskkill` to close unresponsive programs, and `resmon` to monitor resource usage.

- **Maintaining System Health**:
  - Use `chkdsk` and `sfc /scannow` to check for and repair disk and system file issues.

---

Keep this cheat sheet handy as you navigate the Windows command line. Practice these commands to become more comfortable and efficient in managing your Windows system.