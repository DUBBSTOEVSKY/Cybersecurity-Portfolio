# Introduction to Linux

## History

Picture this: It's the 1970s. Ken Thompson and Dennis Ritchie from AT&T create Unix, the granddaddy of operating systems. Fast forward to 1991, a Finnish student named Linus Torvalds decides to make his own OS, probably because he was bored or just wanted to out-nerd everyone. This project grew into what we know today as the Linux kernel, the heart of countless distributions (distros) like Ubuntu, Fedora, and the beloved Linux Mint. 

Linux is everywhere—from your phone to your TV to that WiFi router you constantly have to reboot. It's like the secret sauce in your tech burger.

## Philosophy

Linux follows some zen-like principles:

1. **Everything is a File**: Yep, even your cat photos.
2. **Small, Single-Purpose Programs**: Think of them as highly specialized kitchen gadgets.
3. **Chain Programs Together**: Like making a Rube Goldberg machine but way cooler.
4. **Avoid Captive User Interfaces**: It’s all about that terminal life—feeling like a hacker yet?
5. **Config Data in Text Files**: Ever wonder why you’re always editing some `.conf` file? Now you know.

## Components

- **Bootloader**: The magic that wakes up your computer.
- **OS Kernel**: The mastermind orchestrating everything, kind of like the conductor in an orchestra.
- **Daemons**: Background minions doing the boring stuff.
- **OS Shell**: Your command line sidekick.
- **Graphics Server**: Makes the pretty pictures happen.
- **Window Manager**: The boss of the graphical user interface (GUI) gang.
- **Utilities**: The handy apps and tools making life easier.

## Linux Architecture

Think of Linux as a layer cake:

1. **Hardware**: The bottom layer—RAM, CPU, etc.
2. **Kernel**: The cake itself, managing all the goodies.
3. **Shell**: The frosting, where you interact.
4. **System Utility**: The sprinkles, adding extra functionality.

## File System Hierarchy

Linux's directory structure is like a tree with many branches:

- **/**: The root of all things.
- **/bin**: Essential commands, like your morning coffee.
- **/boot**: Gets the OS up and running.
- **/dev**: Talks to your devices.
- **/etc**: Configuration central.
- **/home**: Your personal playground.
- **/lib**: Shared libraries, because sharing is caring.
- **/media**: Mounts external stuff.
- **/mnt**: Temporary mounting.
- **/opt**: Third-party treasures.
- **/root**: The root user’s lair.
- **/sbin**: System admin tools.
- **/tmp**: Temporary files (cleanup on reboot).
- **/usr**: User-related stuff.
- **/var**: Logs, emails, and other changeable data.

## Using Parrot OS

In our Linux adventures, we'll be using Parrot OS, a Debian-based distro focusing on security and privacy. It's like having a Swiss Army knife in your digital toolbox.

## Conclusion

Welcome to the wild world of Linux! It's powerful, flexible, and a bit quirky—just like you after a few cups of coffee. Dive in, have fun, and remember: when in doubt, there's always a man page to read.


# System Information

## Introduction

When diving into the Linux world, understanding your system is crucial. Think of it as getting to know the controls of your spaceship before you start exploring the galaxy. Here, we'll go over essential commands to help you gather vital system information.

## Essential Commands

- **`whoami`**: Think of it as looking in a mirror. It tells you who you are on the system.
  
  ```bash
  $ whoami
  cry0l1t3
  ```

- **`id`**: Like checking your ID card. It shows your user ID and group memberships.
  
  ```bash
  $ id
  uid=1000(cry0l1t3) gid=1000(cry0l1t3) groups=1000(cry0l1t3),1337(hackthebox)
  ```

- **`hostname`**: This tells you your computer's name. It’s like asking your spaceship's AI its name.
  
  ```bash
  $ hostname
  nixfund
  ```

- **`uname`**: Provides detailed system information, like your spaceship's specs.
  
  ```bash
  $ uname -a
  Linux box 4.15.0-99-generic #100-Ubuntu SMP x86_64 GNU/Linux
  ```

- **`ifconfig`** and **`ip`**: These commands reveal your network interface details. Imagine them as your communication system's diagnostics.

  ```bash
  $ ifconfig
  ```

  ```bash
  $ ip addr
  ```

- **`netstat`** and **`ss`**: Show network status and socket information. Think of these as monitoring your ship’s communication logs.

  ```bash
  $ netstat
  ```

  ```bash
  $ ss
  ```

- **`ps`**: Displays process status. Like checking the crew's activities on your spaceship.

  ```bash
  $ ps
  ```

- **`lsblk`**: Lists block devices, akin to seeing all your spaceship's storage compartments.

  ```bash
  $ lsblk
  ```

- **`lsusb`**: Lists USB devices, like cataloging your connected gadgets.

  ```bash
  $ lsusb
  ```

- **`lspci`**: Lists PCI devices, similar to an inventory of your ship’s internal components.

  ```bash
  $ lspci
  ```

## Practical Examples

### Hostname

Using the `hostname` command is straightforward.

```bash
$ hostname
nixfund
```

### Whoami

After gaining access to a system, `whoami` helps you identify your current user.

```bash
$ whoami
cry0l1t3
```

### Id

The `id` command gives you more detailed user information.

```bash
$ id
uid=1000(cry0l1t3) gid=1000(cry0l1t3) groups=1000(cry0l1t3),1337(hackthebox)
```

### Uname

To get a comprehensive view of your system, `uname -a` is your go-to command.

```bash
$ uname -a
Linux box 4.15.0-99-generic #100-Ubuntu SMP x86_64 GNU/Linux
```

### Uname to Obtain Kernel Release

To quickly check for potential kernel exploits, use `uname -r`.

```bash
$ uname -r
4.15.0-99-generic
```

## Conclusion

Learning these commands is like mastering the controls of your spaceship. With this knowledge, you can navigate through the Linux universe with confidence. Remember, these tools not only help you manage your system but also uncover vulnerabilities and optimize performance. Happy exploring, and may the source be with you!