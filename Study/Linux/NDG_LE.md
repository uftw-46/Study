# NDG Linux Essentials — Organized Course Notes

> A structured Markdown edition of the supplied course material. The original course terminology and examples are retained wherever possible. Image references and image-only descriptions have been removed; command examples and technical text remain.

## How to use these notes

- Use the table of contents to jump to a topic.
- Commands and paths are written in inline code or code blocks where practical.
- Pay attention to differences between commands, options, file paths, and shell metacharacters.
- The source material contains topics in the course's original numbering order, which is not always sequential. The numbering has been preserved rather than silently renumbered.

## Table of contents

  - [1.1 — Linux is Everywhere](#11-linux-is-everywhere)
  - [1.2 — Linux is a Kernel](#12-linux-is-a-kernel)
  - [1.3 — Linux is Open Source](#13-linux-is-open-source)
  - [1.4 — Linux Has Distributions](#14-linux-has-distributions)
  - [1.5 — Linux Embraces the CLI](#15-linux-embraces-the-cli)
  - [2.1 — Operating Systems](#21-operating-systems)
    - [2.1.1 — Decision Points](#211-decision-points)
  - [2.2 — Microsoft Windows](#22-microsoft-windows)
  - [2.3 — Apple macOS](#23-apple-macos)
  - [2.4 — Linux](#24-linux)
- [212 — packages can be updated.](#212-packages-can-be-updated)
- [91 — updates are security updates.](#91-updates-are-security-updates)
    - [2.4.1 — Linux Distributions](#241-linux-distributions)
    - [2.4.2 — Embedded Systems](#242-embedded-systems)
  - [3.1 — Navigating the Linux Desktop](#31-navigating-the-linux-desktop)
    - [3.1.1 — Getting to the Command Line](#311-getting-to-the-command-line)
  - [3.2 — Applications](#32-applications)
  - [5.1 — Introduction](#51-introduction)
  - [5.2 — Shell](#52-shell)
  - [5.4 — Variables](#54-variables)
    - [5.4.1 — Local Variables](#541-local-variables)
    - [5.4.2 — Environment Variables](#542-environment-variables)
- [500 — ](#500)
    - [5.4.3 — Path Variable](#543-path-variable)
  - [5.5 — Command Types](#55-command-types)
    - [5.5.2 — External Commands](#552-external-commands)
    - [5.5.3 — Aliases](#553-aliases)
- [2019 — ](#2019)
- [1 — 2 3 4 5 1 2 1 2](#1-2-3-4-5-1-2-1-2)
- [6 — 7 8 9 10 11 12 3 4 5 6 7 8 9 3 4 5 6 7 8 9](#6-7-8-9-10-11-12-3-4-5-6-7-8-9-3-4-5-6-7-8-9)
- [13 — 14 15 16 17 18 19 10 11 12 13 14 15 16 10 11 12 13 14 15 16](#13-14-15-16-17-18-19-10-11-12-13-14-15-16-10-11-12-13-14-15-16)
- [20 — 21 22 23 24 25 26 17 18 19 20 21 22 23 17 18 19 20 21 22 23](#20-21-22-23-24-25-26-17-18-19-20-21-22-23-17-18-19-20-21-22-23)
- [27 — 28 29 30 31 24 25 26 27 28 24 25 26 27 28 29 30](#27-28-29-30-31-24-25-26-27-28-24-25-26-27-28-29-30)
    - [5.5.4 — Functions](#554-functions)
  - [5.6 — Quoting](#56-quoting)
    - [5.6.1 — Double Quotes](#561-double-quotes)
    - [5.6.2 — Single Quotes](#562-single-quotes)
    - [5.6.3 — Backslash Character](#563-backslash-character)
    - [5.6.4 — Backquotes](#564-backquotes)
  - [5.7 — Control Statements](#57-control-statements)
    - [5.7.1 — Semicolon](#571-semicolon)
- [1 — 2 3 4 5](#1-2-3-4-5)
- [6 — 7 8 9 10 11 12](#6-7-8-9-10-11-12)
- [13 — 14 15 16 17 18 19](#13-14-15-16-17-18-19)
- [20 — 21 22 23 24 25 26](#20-21-22-23-24-25-26)
- [27 — 28 29 30 31](#27-28-29-30-31)
- [1 — 2](#1-2)
- [3 — 4 5 6 7 8 9](#3-4-5-6-7-8-9)
- [10 — 11 12 13 14 15 16](#10-11-12-13-14-15-16)
- [17 — 18 19 20 21 22 23](#17-18-19-20-21-22-23)
- [24 — 25 26 27 28](#24-25-26-27-28)
- [1 — 2](#1-2)
- [3 — 4 5 6 7 8 9](#3-4-5-6-7-8-9)
- [10 — 11 12 13 14 15 16](#10-11-12-13-14-15-16)
- [17 — 18 19 20 21 22 23](#17-18-19-20-21-22-23)
- [24 — 25 26 27 28 29 30](#24-25-26-27-28-29-30)
- [31 — ](#31)
    - [5.7.2 — Double Ampersand](#572-double-ampersand)
    - [5.7.3 — Double Pipe](#573-double-pipe)
  - [4.1 — Introduction](#41-introduction)
  - [4.2 — Open Source Licensing](#42-open-source-licensing)
    - [4.2.1 — The Free Software Foundation](#421-the-free-software-foundation)
    - [4.2.2 — The ‌⁠​​⁠​ Open Source Initiative](#422-the-open-source-initiative)
    - [4.2.3 — Creative Commons](#423-creative-commons)
  - [4.3 — Open Source Business Models](#43-open-source-business-models)
  - [6.1 — Introduction](#61-introduction)
  - [6.2 — Man Pages](#62-man-pages)
    - [6.2.1 — Viewing Man Pages](#621-viewing-man-pages)
    - [6.2.2 — Sections Within Man Pages](#622-sections-within-man-pages)
    - [6.2.4 — Man Pages Categorized by Sections](#624-man-pages-categorized-by-sections)
  - [6.3 — Finding Commands and Documentation](#63-finding-commands-and-documentation)
  - [6.4 — Info Documentation](#64-info-documentation)
  - [7.1 — Introduction](#71-introduction)
  - [7.2 — Directory Structure](#72-directory-structure)
    - [7.2.1 — Home Directory](#721-home-directory)
    - [7.2.2 — Current Directory](#722-current-directory)
    - [7.2.3 — Changing Directories](#723-changing-directories)
  - [7.3 — Paths](#73-paths)
  - [7.4 — Listing Files in a Directory](#74-listing-files-in-a-directory)
  - [8.1 — Introduction](#81-introduction)
  - [8.2 — Globbing](#82-globbing)
    - [8.2.1 — Asterisk * Character](#821-asterisk-character)
    - [8.2.2 — Question Mark ? Character](#822-question-mark-character)
    - [8.2.3 — Bracket [ ] Characters](#823-bracket-characters)
    - [8.2.4 — Exclamation Point ! Character](#824-exclamation-point-character)
    - [8.2.5 — Listing With Globs](#825-listing-with-globs)
  - [8.3 — Copying Files](#83-copying-files)
  - [8.4 — Moving Files](#84-moving-files)
  - [8.5 — Creating Files](#85-creating-files)
  - [8.6 — Removing Files](#86-removing-files)
  - [8.7 — Creating Directories](#87-creating-directories)
  - [10.1 — Introduction](#101-introduction)
    - [10.1.1 — Viewing Files in the Terminal](#1011-viewing-files-in-the-terminal)
    - [10.1.2 — Viewing Files Using a Pager](#1012-viewing-files-using-a-pager)
      - [10.1.2.1 — Pager Movement Commands](#10121-pager-movement-commands)
  - [10.2 — Command Line Pipes](#102-command-line-pipes)
- [1 — moduli](#1-moduli)
- [2 — ssh_config](#2-ssh_config)
- [3 — ssh_host_ecdsa_key](#3-ssh_host_ecdsa_key)
- [4 — ssh_host_ecdsa_key.pub](#4-ssh_host_ecdsa_keypub)
- [5 — ssh_host_ed25519_key](#5-ssh_host_ed25519_key)
- [6 — ssh_host_ed25519_key.pub](#6-ssh_host_ed25519_keypub)
- [7 — ssh_host_rsa_key](#7-ssh_host_rsa_key)
- [8 — ssh_host_rsa_key.pub](#8-ssh_host_rsa_keypub)
- [9 — ssh_import_id](#9-ssh_import_id)
- [10 — sshd_config](#10-sshd_config)
- [6 — ssh_host_ed25519_key.pub](#6-ssh_host_ed25519_keypub)
- [7 — ssh_host_rsa_key](#7-ssh_host_rsa_key)
- [8 — ssh_host_rsa_key.pub](#8-ssh_host_rsa_keypub)
- [9 — ssh_import_id](#9-ssh_import_id)
- [10 — sshd_config](#10-sshd_config)
- [1 — ssh_host_ed25519_key.pub](#1-ssh_host_ed25519_keypub)
- [2 — ssh_host_rsa_key](#2-ssh_host_rsa_key)
- [3 — ssh_host_rsa_key.pub](#3-ssh_host_rsa_keypub)
- [4 — ssh_import_id](#4-ssh_import_id)
- [5 — sshd_config](#5-sshd_config)
  - [10.3 — Input/Output Redirection](#103-inputoutput-redirection)
  - [10.4 — Sorting Files or Input](#104-sorting-files-or-input)
    - [10.4.1 — Fields and Sort Options](#1041-fields-and-sort-options)
  - [10.5 — Viewing File Statistics](#105-viewing-file-statistics)
- [35 — 56 1710 /etc/passwd](#35-56-1710-etcpasswd)
- [34 — 55 1665 /etc/passwd-](#34-55-1665-etcpasswd-)
- [69 — 111 3375 total](#69-111-3375-total)
  - [10.6 — Filter File Sections](#106-filter-file-sections)
  - [10.7 — Filter File Contents](#107-filter-file-contents)
  - [10.8 — Basic Regular Expressions](#108-basic-regular-expressions)
    - [10.8.1 — The Period . Character](#1081-the-period-character)
    - [10.8.6 — Extended Regular Expressions](#1086-extended-regular-expressions)
  - [11.1 — Introduction](#111-introduction)
  - [11.2 — Shell Scripts in a Nutshell](#112-shell-scripts-in-a-nutshell)
  - [11.3 — Editing Shell Scripts](#113-editing-shell-scripts)
  - [11.4 — Scripting Basics](#114-scripting-basics)
  - [12.1 — Introduction](#121-introduction)
  - [12.2 — Motherboards](#122-motherboards)
  - [12.3 — Processors](#123-processors)
  - [12.4 — Random Access Memory](#124-random-access-memory)
  - [12.5 — Buses](#125-buses)
  - [12.6 — Hard Drives](#126-hard-drives)
- [255 — heads, 63 sectors/track, 2610 cylinders, total 41943040 sectors](#255-heads-63-sectorstrack-2610-cylinders-total-41943040-sectors)
  - [12.7 — Solid State Disks](#127-solid-state-disks)
  - [12.8 — Optical Drives](#128-optical-drives)
  - [12.9 — Managing Devices](#129-managing-devices)
  - [12.10 — Video Display Devices](#1210-video-display-devices)
  - [12.11 — Power Supplies](#1211-power-supplies)
  - [14.1 — Introduction](#141-introduction)
  - [14.2 — Basic Network Terminology](#142-basic-network-terminology)
  - [14.3 — Networking Features Terminology](#143-networking-features-terminology)
  - [14.4 — IP Addresses](#144-ip-addresses)
  - [14.5 — Configuring Network Devices](#145-configuring-network-devices)
      - [14.5.1.1 — Primary IPv4 Configuration File](#14511-primary-ipv4-configuration-file)
      - [14.5.1.2 — Primary IPv6 Configuration File](#14512-primary-ipv6-configuration-file)
      - [14.5.1.3 — Domain Name System (DNS)](#14513-domain-name-system-dns)
      - [14.5.1.4 — Network Configuration Files](#14514-network-configuration-files)
      - [127.0.0.1 — localhost](#127001-localhost)
  - [14.6 — Network Tools](#146-network-tools)
    - [14.6.1 — The ifconfig Command](#1461-the-ifconfig-command)
    - [14.6.2 — The ip Command](#1462-the-ip-command)
    - [14.6.3 — The route Command](#1463-the-route-command)
      - [192.168.1.0 — * 255.255.255.0 U 0 0 0 eth0](#19216810-2552552550-u-0-0-0-eth0)
      - [192.168.1.0 — 0.0.0.0 255.255.255.0 U 0 0 0 eth0](#19216810-0000-2552552550-u-0-0-0-eth0)
      - [0.0.0.0 — 192.168.1.1 0.0.0.0 UG 0 0 0 eth0](#0000-19216811-0000-ug-0-0-0-eth0)
    - [14.6.4 — The ping Command](#1464-the-ping-command)
- [64 — bytes from 192.168.1.2: icmp_req=1 ttl=64 time=0.051 ms](#64-bytes-from-19216812-icmp_req1-ttl64-time0051-ms)
- [64 — bytes from 192.168.1.2: icmp_req=2 ttl=64 time=0.064 ms](#64-bytes-from-19216812-icmp_req2-ttl64-time0064-ms)
- [64 — bytes from 192.168.1.2: icmp_req=3 ttl=64 time=0.050 ms](#64-bytes-from-19216812-icmp_req3-ttl64-time0050-ms)
- [64 — bytes from 192.168.1.2: icmp_req=4 ttl=64 time=0.043 ms](#64-bytes-from-19216812-icmp_req4-ttl64-time0043-ms)
- [4 — packets transmitted, 4 received, 0% packet loss, time 2999ms](#4-packets-transmitted-4-received-0-packet-loss-time-2999ms)
- [4 — packets transmitted, 0 received, +4 errors, 100% packet loss, time 2999ms](#4-packets-transmitted-0-received-4-errors-100-packet-loss-time-2999ms)
    - [14.6.5 — The netstat Command](#1465-the-netstat-command)
      - [192.168.1.0 — * 255.255.255.0 U 0 0 0 eth0](#19216810-2552552550-u-0-0-0-eth0)
    - [14.6.6 — The ss Command](#1466-the-ss-command)
    - [14.6.7 — The dig Command](#1467-the-dig-command)
    - [14.6.8 — The host Command](#1468-the-host-command)
    - [14.6.9 — The ssh Command](#1469-the-ssh-command)
      - [14.6.9.1 — RSA Key Fingerprint](#14691-rsa-key-fingerprint)
  - [17.1 — Introduction](#171-introduction)
  - [17.2 — File Ownership](#172-file-ownership)
  - [17.3 — Changing Groups](#173-changing-groups)
  - [17.4 — Changing Group Ownership](#174-changing-group-ownership)
  - [17.4 — Changing Group Ownership](#174-changing-group-ownership)
  - [17.6 — Permissions](#176-permissions)
  - [17.7 — Understanding Permissions](#177-understanding-permissions)
  - [17.8 — Changing Permissions](#178-changing-permissions)
  - [17.9 — Default Permissions](#179-default-permissions)
  - [18.1 — Introduction](#181-introduction)
  - [18.2 — Setuid](#182-setuid)
  - [18.3 — Setgid](#183-setgid)
    - [18.3.1 — Setgid on Files](#1831-setgid-on-files)
    - [18.3.2 — Setgid on Directories](#1832-setgid-on-directories)
    - [18.3.3 — Setting Setgid](#1833-setting-setgid)
  - [18.4 — Sticky Bit](#184-sticky-bit)
  - [18.5 — Links](#185-links)
    - [18.5.1 — Creating Hard Links](#1851-creating-hard-links)
- [215220874 — /tmp/file.txt](#215220874-tmpfiletxt)
- [278772 — -rw-rw-r--. 1 sysadmin sysadmin 5 Oct 25 15:42 file.original](#278772--rw-rw-r---1-sysadmin-sysadmin-5-oct-25-1542-fileoriginal)
- [278772 — -rw-rw-r--. 2 sysadmin sysadmin 5 Oct 25 15:53 file.hard.1](#278772--rw-rw-r---2-sysadmin-sysadmin-5-oct-25-1553-filehard1)
- [278772 — -rw-rw-r--. 2 sysadmin sysadmin 5 Oct 25 15:53 file.original](#278772--rw-rw-r---2-sysadmin-sysadmin-5-oct-25-1553-fileoriginal)
    - [18.5.2 — Creating Symbolic Links](#1852-creating-symbolic-links)
    - [18.5.3 — Comparing Hard and Symbolic Links](#1853-comparing-hard-and-symbolic-links)
- [278772 — file.original](#278772-fileoriginal)
  - [16.1 — Introduction](#161-introduction)
  - [16.2 — Groups](#162-groups)
  - [16.3 — Users](#163-users)
  - [15.1 — Introduction](#151-introduction)
  - [15.2 — Administrative Accounts](#152-administrative-accounts)
  - [15.3 — User Accounts](#153-user-accounts)
  - [15.4 — System Accounts](#154-system-accounts)
  - [15.5 — Group Accounts](#155-group-accounts)
  - [15.6 — Viewing User Information](#156-viewing-user-information)
- [1001 — 4 27](#1001-4-27)
  - [15.7 — Viewing Current Users](#157-viewing-current-users)
  - [15.8 — Viewing Login History](#158-viewing-login-history)
  - [15.8 — Viewing Login History](#158-viewing-login-history)
  - [13.2 — Processes](#132-processes)
- [1 — cpuinfo irq modules sys](#1-cpuinfo-irq-modules-sys)
- [128 — crypto kallsyms mounts sysrq-trigger](#128-crypto-kallsyms-mounts-sysrq-trigger)
- [17 — devices kcore mtrr sysvipc](#17-devices-kcore-mtrr-sysvipc)
- [21 — diskstats key-users net thread-self](#21-diskstats-key-users-net-thread-self)
- [23 — dma keys pagetypeinfo timer_list](#23-dma-keys-pagetypeinfo-timer_list)
- [39 — driver kmsg partitions timer_stats](#39-driver-kmsg-partitions-timer_stats)
- [60 — execdomains kpagecgroup sched_debug tty](#60-execdomains-kpagecgroup-sched_debug-tty)
- [72 — fb kpagecount schedstat uptime](#72-fb-kpagecount-schedstat-uptime)
- [64 — bytes from localhost.localdomain (127.0.0.1): icmp_seq=1 ttl=64 time=0.026 ms](#64-bytes-from-localhostlocaldomain-127001-icmp_seq1-ttl64-time0026-ms)
- [1 — packets transmitted, 1 received, 0% packet loss, time 0ms](#1-packets-transmitted-1-received-0-packet-loss-time-0ms)
- [1 — packets transmitted, 0 received, 100% packet loss, time 10000ms](#1-packets-transmitted-0-received-100-packet-loss-time-10000ms)
  - [13.3 — Memory](#133-memory)
  - [13.4 — Log Files](#134-log-files)
  - [13.5 — Kernel Messages](#135-kernel-messages)
  - [13.6 — Filesystem Hierarchy Standard](#136-filesystem-hierarchy-standard)
    - [13.6.1 — Organization Within the Filesystem Hierarchy](#1361-organization-within-the-filesystem-hierarchy)

---

### 1.1 Linux is Everywhere

Hello and welcome to NDG Linux Essentials!

```text
Linux is everywhere; Linux jobs are everywhere. There is a demand for Linux skills in just about every industry and job category on the planet, and not enough Linux talent to meet this growing demand. It’s also fun and rewarding to work with something that’s so much a part of our modern lives yet which so few people understand.
```

If someone says they have Linux experience, it might refer to configuring systems, running web servers, or any number of other services and programs that operate on top of Linux. Over time, Linux administration has evolved to encompass just about every task that a modern business, educational institution or government organization might use in their daily operations.
The journey of learning you are beginning today has no ending point. It can take you in a myriad of different directions, from cybersecurity to application and game development, system administration, networking, big data, and artificial intelligence; all of these fields are rooted in Linux.
Every time you execute a search on the internet, watch a video on your phone or order something online, that’s likely Linux at work. It epitomizes a whole that is greater than the sum of its parts, a vast undertaking, done voluntarily, by some of the smartest people on the planet.
While your journey will be ongoing, be comforted that you are learning a set of technologies, commands, and methods that have stood the test of time. Linux utilizes and expands upon many of the commands and ways of accomplishing computing that UNIX began, with a rate of change per year that’s very manageable. Now, some 30+ years on, many of those learned commands are still active and used every day by sysadmins, devops, and architects. Linux is a revolution of evolution, allowing you to learn the majority once and keep up with the small percentage of changes in a continual learning process.

### 1.2 Linux is a Kernel

The definition of the word Linux depends on the context in which it is used. Linux means the kernel of the system, which is the central controller of everything that happens on the computer.
When most people refer to Linux, they are really referring to a combination of software called GNU/Linux, which defines the operating system. GNU is the free software that provides open source equivalents of many common UNIX commands. The Linux part of this combination is the Linux kernel, which is the core of the operating system. The kernel is loaded at boot time and stays running to manage every aspect of the functioning system.
The story of Linux begins with UNIX, an operating system developed at AT&T Bell Labs in the 1970s. UNIX is written in the C language making it uniquely portable amongst competing operating systems, which were typically closely tied to the hardware for which they were written. It quickly gained popularity in research and academic settings, as well as amongst programmers who were attracted to its modularity. Over time it was modified and forked (that is, people modified it, and those modifications served as the basis for other systems) such that at present there are many different variants of UNIX. However, UNIX is now both a trademark and a specification, owned by an industry consortium called the Open Group. Only software that has been certified by the Open Group may call itself UNIX.

```text
Linux started in 1991 as a hobby project of Linus Torvalds, a Finnish-born computer scientist studying at the University of Helsinki. Frustrated by the licensing of MINIX, a UNIX-like operating system designed for educational use, and its creator’s desire not to make it a full operating system, Linus decided to create his own OS kernel.
```

From this humble beginning, Linux has grown to be the dominant operating system on the Internet, and arguably the most important computer program of any kind. Despite adopting all the requirements of the UNIX specification, Linux has not been certified, so Linux really isn’t UNIX! It’s just... UNIX-like.
Prior to and alongside this development was the GNU Project, created by Richard Stallman in 1983. While GNU initially focused on building their own operating system, they ultimately were far more effective at building tools that go along with a UNIX-like operating system, such as the editors, compilers and user interfaces that make a kernel usable. Since the source was all freely available, Linux programmers were able to incorporate the GNU tools to provide a complete operating system. As such, many of the tools and utilities that are part of the Linux system evolved from these early GNU tools.

> **Consider This**
>
Linus originally named the project Freax, however, an administrator of the server where the development files were uploaded renamed it Linux, a portmanteau of Linus’ name and UNIX. The name stuck.
GNU is a recursive acronym for “GNU’s Not Unix,” and it’s pronounced just like the African horned antelope that is its namesake.

### 1.3 Linux is Open Source

Historically, most software has been issued under a closed-source license, meaning that you get the right to use the machine code, but cannot see the source code. Often the license explicitly says that you may not attempt to reverse engineer the machine code back to source code to figure out what it does!
The development of Linux closely parallels the rise of open source software. Open source takes a source-centric view of software. The open source philosophy is that you have a right to obtain the software source code and to modify it for your own use.

```text
Linux adopted this philosophy to great success. Linus made the source programming code (the instructions a computer uses to operate) freely available, allowing others to join in and shape this fledgling operating system. It was not the first system to be developed by a volunteer group, but since it was built from scratch, early adopters could influence the project’s direction. People took the source, made changes, and shared them back with the rest of the group, greatly accelerating the pace of development, and ensuring mistakes from other operating systems were not repeated.

> **Consider This**
>
```

The source code may be written in any of hundreds of different languages. Linux happens to be written in C, a versatile and relatively easy language to learn, which shares history with the original UNIX. This decision, made long before it’s utility was proven, turned out to be crucial in its nearly universal adoption as the primary operating system for internet servers.

### 1.4 Linux Has Distributions

People that say their computer runs Linux usually refer to the kernel, tools, and suite of applications that come bundled together in what is referred to as a distribution.
Take Linux and the GNU tools, add some user-facing applications like a web browser and an email client, and you have a full Linux system. Individuals and even companies started bundling all this software into distributions almost as soon as Linux became usable. The distribution includes tools that take care of setting up the storage, installing the kernel, and installing the rest of the software. The full-featured distributions also include tools to manage the system and a package manager to help you add and remove software after the installation is complete.
Like UNIX, there are distributions suited to every imaginable purpose. There are distributions that focus on running servers, desktops, or even industry-specific tools such as electronics design or statistical computing. The major players in the market can be traced back to either Red Hat, Debian or Slackware. The most visible difference between Red Hat and Debian derivatives is the package manager though there are other differences in everything from file locations to political philosophies.

### 1.5 Linux Embraces the CLI

There are two basic types of interfaces available that allow you to interact with the operating system. The typical computer user today is most familiar with a graphical user interface (GUI). In a GUI, applications present themselves in windows that can be resized and moved around. There are menus and tools to help users navigate. Graphical applications include web browsers, graphics editing tools and email, to name a few.

The second type of interface is the command line interface (CLI), a text-based interface to the computer. The CLI relies primarily on keyboard input. Everything the user wants the computer to do is relayed by typing commands rather than clicking on icons. It can be said that when a user clicks on an icon, the computer is telling the user what to do, but, when the user types a command, they are telling the computer what to do.

Typically operating systems offer both GUI and CLI interfaces. However, most consumer operating systems (Windows, macOS) are designed to shield the user from the complexity of the CLI. The Linux community is different in that it positively celebrates the CLI for its power, speed and ability to accomplish a vast array of tasks with a single command line instruction. The virtual machines used for the chapters and labs in this course provide a CLI for you to practice on without fear of damaging anything.
When a user first encounters the CLI, they can find it challenging because it requires memorizing a dizzying amount of commands and their options. However, once a user has learned the structure of how commands are used, where the necessary files and directories are located and how to navigate the hierarchy of a filesystem, they can be immensely productive. This capability provides more precise control, greater speed and the ability to easily automate tasks through scripting.
Furthermore, by learning the CLI, a user can easily be productive almost instantly on ANY distribution of Linux, reducing the amount of time needed to familiarize themselves with a system because of variations in a GUI.

### 2.1 Operating Systems

An operating system is software that runs on a computing device and manages the hardware and software components that make up a functional computing system.
Modern operating systems don’t just manage hardware and software resources, they schedule programs to run in a multi-tasking manner (sharing the processor so that multiple tasks can occur apparently simultaneously), provide standard services that allow users and programs to request something happen (for example a print job) from the operating system, and provided it’s properly requested, the operating system will accept the request and perform the function needed.
Desktop and server operating systems are by nature more complex than an operating system that runs on a single-purpose device such as a firewall, or a mobile phone. From a simple set-top box that provides a menu interface for a cable provider, to supercomputers and massive, parallel computing clusters, the generic term operating system is used to describe whatever software is booted and run on that device.

Computer users today have a choice mainly between three major operating systems: Microsoft Windows, Apple macOS, and Linux.
Of the three major operating systems listed only Microsoft Windows is unique in its underlying code. Apple’s macOS is a fully-qualified UNIX distribution based on BSD Unix (an operating system distributed until 1995), complemented by a large amount of proprietary code. It runs on hardware specifically optimized to work with Apple software. Linux can be any one of hundreds of distribution packages designed or optimized for whatever task is required. Only Microsoft Windows is based on a proprietary code base that isn’t either UNIX- or Linux-based.
A user can easily interact with any of these systems by pointing and clicking their way through everyday productivity tasks that all behave similarly regardless of the underlying operating system. Except for Windows, which is mostly administered via the GUI, most system administration tasks are performed using typed commands in a terminal. An administrator that is familiar with UNIX can typically perform tasks on a Linux system and vice versa. Many Linux command line functions also have Microsoft equivalents that administrators use to do their work efficiently.

#### 2.1.1 Decision Points

Role
The first decision when specifying any computer system is the machine’s role. Will you be sitting at the console running productivity applications or web browsing? If so, a familiar desktop is best. Will the machine be accessed remotely by many users or provide services to remote users? Then it’s a server.
Servers typically sit in a rack and share a keyboard and monitor with many other computers, since console access is generally only used for configuration and troubleshooting. Servers generally run as a CLI, which frees up resources for the real purpose of the computer: serving information to clients (any user or system that accesses resources remotely). Desktop systems primarily run a GUI for the ease of use of their users.
Function
Next, determine the functions of the machine. Is there specific software it needs to run, or specific functions it needs to perform? Will there be hundreds, even thousands, of these machines running at the same time? What is the skill-set of the team managing the computer and software?
Life Cycle
The service lifetime and risk tolerance of the server also needs to be determined. Operating systems and software upgrades come on a periodic basis, called a release cycle. Vendors only support older versions of software for a certain period of time before not offering any updates; this is called a maintenance cycle or life cycle.
In an enterprise server environment, maintenance and release cycles are critical considerations because it is time-consuming and expensive to do major upgrades. Instead, the server hardware itself is often replaced because increased performance is worth the extra expense, and the resources involved are often many times more costly than the hardware.

> **Consider This**
>
There is a fair amount of work involved in upgrading a server due to specialized configurations, application software patching and user testing, so a proactive organization will seek to maximize their return on investment in both human and monetary capital.
Modern data centers are addressing this challenge through virtualization. In a virtual environment, one physical machine can host dozens, or even hundreds of virtual machines, decreasing space and power requirements, as well as providing for automation of many of the tasks previously done manually by systems administrators. Scripting programs allow virtual machines to be created, configured, deployed and removed from a network without the need for human intervention. Of course, a human still needs to write the script and monitor these systems, at least for now.
The need for physical hardware upgrades has also been decreased immensely with the advent of cloud services providers like Amazon Web Services, Rackspace, and Microsoft Azure. Similar advances have helped desktop administrators manage upgrades in an automated fashion and with little to no user interruption.
‌⁠​​⁠​Stability
Individual software releases can be characterized as beta or stable depending on where they are in the release cycle. When a software release has many new features that haven’t been tested, it’s typically referred to as beta. After being tested in the field, its designation changes to stable.
Users who need the latest features can decide to use beta software. This is often done in the development phase of a new deployment and provides the ability to request features not available on the stable release.
Production servers typically use stable software unless needed features are not available, and the risk of running code that has not been thoroughly tested is outweighed by the utility provided.
Software in the open source realm is often released for peer review very early on in its development process, and can very quickly be put into testing and even production environments, providing extremely useful feedback and code submissions to fix issues found or features needed.
Conversely, proprietary software will often be kept secret for most of its development, only reaching a public beta stage when it’s almost ready for release.
Compatibility
Another loosely-related concept is backward compatibility which refers to the ability of later operating systems to be compatible with software made for earlier versions. This is usually a concern when it is necessary to upgrade an operating system, but an application software upgrade is not possible due to cost or lack of availability.
The norm for open source software development is to ensure backward compatibility first and break things only as a last resort. The common practice of maintaining and versioning libraries of functions helps this greatly. Typically, a library that is used by one or more programs is versioned as a new release when significant changes have occurred but also keeps all the functions (and compatibility) of earlier versions that may be hard-coded or referred to by existing software.
Cost
Cost is always a factor when specifying new systems. Microsoft has annual licensing fees that apply to users, servers and other software, as do many other software companies. Ultimately, the choice of operating system will be affected by available hardware, staff resources and skill, cost of purchase, maintenance, and projected future requirements.
Virtualization and outsourced support services offer the modern IT organization the promise of having to pay for only what it uses rather than building in excess capacity. This not only controls costs but offers opportunities for people both inside and outside the organization to provide expertise and value.
Interface
The first electronic computer systems were controlled by means of switches and plugboards similar to those used by telephone operators at the time. Then came punch cards and finally a text-based terminal system similar to the Linux command line interface (CLI) in use today. The graphical user interface (GUI), with a mouse and buttons to click, was pioneered at Xerox PARC (Palo Alto Research Center) in the early 1970s and popularized by Apple Computer in the 1980s.
Today, operating systems offer both GUI and CLI interfaces, however, most consumer operating systems (Windows, macOS) are designed to shield the user from the ins and outs of the CLI.

### 2.2 Microsoft Windows

Microsoft offers different versions of its operating system according to the machine’s role: desktop or server? The desktop version of Windows has undergone various naming schemes with the current version (as of this writing) being simply Windows 11. While new versions of most Linux distributions come out twice a year, around March and September, new versions of Windows tend to be released only every few years. In all, there have been 16 versions of Windows since 1985. Backward compatibility is a priority for Microsoft, even going so far as to bundle virtual machine technology so that users can run older software.
Windows Server currently (as of this writing) is at version 2019 to denote the release date. The server can run a GUI but recently Microsoft, largely as a competitive response to Linux, has made incredible strides in its command line scripting capabilities through PowerShell and Windows Subsystem for Linux (WSL). There is also an optional Desktop Experience package which mimics a standard productivity machine. Microsoft also actively encourages enterprise customers to incorporate its Azure cloud service.

### 2.3 Apple macOS

Apple makes the macOS operating system, which is partially based on software from the FreeBSD project and has undergone UNIX certification. macOS is well known for being “easy to use”, and as such has continued to be favored by users with limited access to IT resources like schools and small businesses. It is also very popular with programmers due to its robust UNIX underpinnings.
On the server side, macOS Server is primarily aimed at smaller organizations. This low-cost addition to macOS desktop allows users to collaborate, and administrators to control access to shared resources. It also provides integration with iOS devices like the iPhone and iPad.
Some large corporate IT departments allow users to choose macOS since users often require less support than standard Microsoft productivity deployments. The continued popularity of macOS has ensured healthy support from software vendors. macOS is also quite popular in the creative industries such as graphics and video production. For many of these users, application choice drives the operating system decision. Apple hardware, being integrated so closely with the operating system, and their insistence on adherence to standards in application programming gives these creative professionals a stable platform to perform many computing-intense functions with fewer concerns about compatibility.

### 2.4 Linux

```text
Linux users typically obtain an operating system by downloading a distribution. A Linux distribution is a bundle of software, typically comprised of the Linux kernel, utilities, management tools, and even some application software in a package which also includes the means to update core software and install additional applications.
```

The distribution takes care of setting up the storage, building the kernel and installing hardware drivers, as well as installing applications and utilities to make a fully functional computer system. The organizations that create distributions also include tools to manage the system, a package manager to add and remove software, as well as update programs to provide security and functionality patches.
The number of Linux distributions available numbers in the hundreds, so the choice can seem daunting at first. However, the decision points are mostly the same as those highlighted for choosing an operating system.
Role
With Linux, there are multiple options to choose from depending on organizational needs. The variety of distributions and accompanying software allows the operating system to be significantly more flexible and customizable. Distributions are available for a much wider variety of systems, from commercial offerings for the traditional server or desktop roles, to specialized distributions designed to turn an old computer into a network firewall; from distributions created to power a supercomputer, to those that enable embedded systems. These might focus on running application or web servers, productivity desktops, point-of-sale systems, or even tools dedicated to electronics design or statistical computing.
Function
Governments and large enterprises may also limit their choices to distributions that offer commercial support because paying for another tier of support may be better than risking extensive outages. For the most part, concerns over security have been addressed through the large open source community, which monitors kernel changes for vulnerabilities and provides bug reporting and fixes at a much larger scale than closed source vendors can achieve.
Support for necessary applications may vary and is, therefore, an additional consideration. Often application vendors choose a subset of distributions to support. Different distributions have different versions of key libraries, and it is difficult for a company to support all these different versions. However, some applications like Firefox and LibreOffice are widely supported and available for all major distributions.
Life Cycle
Most distributions have both major and minor update cycles to introduce new features and fix existing bugs. Additionally, there are development packages where users can contribute code and submit patches for possible inclusion into new releases.

```text
Linux distributions can be broadly classed in two main categories: enthusiast and enterprise. An enthusiast distribution such as openSUSE’s Tumbleweed has a fast update cycle, is not supported for enterprise and may not contain (or drop) features or software in the next version that are in the current one. Red Hat’s Fedora project uses a similar method of development and release cycle, as does Ubuntu Desktop.
```

Enterprise distributions are almost the exact opposite, in that they take care to be stable and consistent, and offer enterprise-grade support for extended periods, anywhere from 5-13 years in the case of SUSE. Enterprise distributions are fewer by far, being offered mainly by Red Hat, Canonical and SUSE.
Application software may be written such that it only supports a specific release of a distribution, requiring users to remain on an older, less secure operating system than they might like. Therefore, some Linux releases are considered to have long-term support (LTS) of 5 years or more while others are only supported for two years or less.
Stability
Some distributions offer stable, testing, and unstable releases. When choosing an unstable release for required features, consideration must be given to the fact that those features may change at any point during the development cycle. When features have been integrated into the system for a long time, with most of the bugs and issues addressed, the software moves through testing into the stable release.
Other releases depend on beta distributions. For instance, the Fedora distribution releases beta or pre-releases of its software ahead of the full release to minimize bugs. Fedora is often considered the community-oriented beta release of RedHat. Features are added and changed in the Fedora release before finding their way into the enterprise-ready RedHat distribution.
openSUSE and its enterprise counterpart SLES (SUSE Linux Enterprise Server) are similar, in that the community edition is used as a testing ground for the features and functions that will eventually be migrated into the enterprise version. Previously somewhat dissimilar, later versions of the openSUSE and SLES distribution codebases are nearly identical, allowing for easier migration of features and code from one to the other.

> **Consider This**
>
The Debian distribution warns users about the pitfalls of using the “sid” (unstable) release with the following warning:
‘"sid" is subject to massive changes and in-place library updates. This can result in a very "unstable" system which contains packages that cannot be installed due to missing libraries, dependencies that cannot be fulfilled, etc. Use it at your own risk!’
Cost
Your chosen Linux distribution itself might be zero cost, but paying for support may be worthwhile depending on organizational needs and capabilities.
Interface
Like most operating systems, Linux can be used in one of two ways: graphical (GUI) and non-graphical (CLI). Below is an example of a graphical desktop, with a menu bar of popular applications to the left, a LibreOffice document being edited in the foreground, and a web browser in the background.

In graphical mode, users can have several different windows with terminal applications (shells) open, which is very helpful when performing tasks on multiple remote computers. Administrators and users can log-in with their username and password through a graphical interface.
The second type of interface, the CLI, is a text-based interface to the computer, where the user types in a command and the computer then executes it. The CLI environment is provided by an application on the computer known as a terminal. ‌⁠​⁠​ The terminal accepts what the user types and passes to a shell. The shell interprets what the user has typed into instructions that can be executed by the operating system. If output is produced by the command, then this text is displayed in the terminal. If problems with the command are encountered, then an error message is displayed.
The CLI starts with a text-based login as shown below. In a successful login, after being prompted for a username and password, you are taken to a CLI shell customized for the particular user.

```text
ubuntu 18.04 ubuntu tty2

ubuntu login:
```

In CLI mode there are no windows to move around. Text editors, web browsers, and email clients are all presented in text format only. This is how UNIX operated before graphical environments were the norm. Most servers run in this mode too, since people don’t log into them directly, making a graphical interface a waste of resources. Here is an example of a CLI screen after logging in:

```text
ubuntu 18.04 ubuntu tty2

ubuntu login: sue
Password:

The programs included with the Ubuntu system are free software;
```

the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

```text
Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
```

applicable law.

```text
Welcome to Ubuntu 18.04 LTS (GNU/Linux 4.4.0-72-generic x86_64)

```

* Documentation:  https://help.ubuntu.com/

## 212 packages can be updated.

## 91 updates are security updates.

```text
sue@ubuntu:~$ w
```

17:27:22 up 14 min,  2 users,  load average: 1.73, 1.83, 1.69

```text
USER     TTY      FROM              LOGIN@   IDLE   JCPU   PCPU WHAT
```

sue    tty2                       20:08    14.35  0.05s  0.00s w
The original login prompt is at the top, with newer text added below. During login there may be some text displayed called the message of the day (MOTD). This is an opportunity for the systems administrator to pass information to users, or just make a silly joke. Following the MOTD is the command prompt, in the example above, the user has entered the w command which shows who is logged in. As new commands are entered and processed, the window scrolls up and older text is lost across the top. The terminal itself is responsible for keeping any history, such as to allow the user to scroll up and see previously entered commands. As far as Linux is concerned, what is on the screen is all that there is. There’s nothing to move around.

#### 2.4.1 Linux Distributions

Red Hat
Red Hat started as a simple distribution that introduced the Red Hat Package Manager (RPM). The developer eventually formed a company around it, which tried to commercialize a Linux desktop for business. Over time, Red Hat started to focus more on the server applications, such as web- and file-serving and released Red Hat Enterprise Linux (RHEL), which was a paid service on a long release cycle. The release cycle dictates how often software is upgraded. A business may value stability and want long release cycles, while a hobbyist or a startup may want the latest software and opt for a shorter release cycle. To satisfy the latter group, Red Hat sponsors the Fedora Project which makes a personal desktop comprising the latest software but is still built on the same foundations as the enterprise version.
Because everything in Red Hat Enterprise Linux is open source, a project called CentOS came to be. It recompiled all the RHEL packages (converting their source code from the programming language they were written into language usable by the system) and gave them away for free. CentOS and others like it (such as Scientific Linux) are largely compatible with RHEL and integrate some newer software, but do not offer the paid support that Red Hat does.
Scientific Linux is an example of a specific-use distribution based on Red Hat. The project is a Fermilab-sponsored distribution designed to enable scientific computing. Among its many applications, Scientific Linux is used with particle accelerators including the Large Hadron Collider at CERN.
SUSE
SUSE, originally derived from Slackware, was one of the first comprehensive Linux distributions, it has many similarities to Red Hat Enterprise Linux. The original company was purchased by Novell in 2003, which was then purchased by the Attachmate Group in 2011. The Attachmate group then merged with Micro Focus International in 2014, and in 2018 SUSE announced plans to go forward as an independent business. Through all of the mergers and acquisitions, SUSE has managed to continue and grow.
While SUSE Linux Enterprise contains proprietary code and is sold as a server product, openSUSE is a completely open, free version with multiple desktop packages similar to CentOS and Linux Mint.
Debian
Debian is more of a community effort, and as such, also promotes the use of open source software and adherence to standards. Debian came up with its own package management system based on the .deb file format. While Red Hat leaves non-Intel and AMD platform support to derivative projects, Debian supports many of these platforms directly.
Ubuntu is the most popular Debian-derived distribution. It is the creation of Canonical, a company that was made to further the growth of Ubuntu and makes money by providing support. Ubuntu has several different variants for desktop, server and various specialized applications. They also offer an LTS version that is kept up-to-date for 3 years on desktops and 5 years on servers, which gives developers and the companies they work for confidence to build solutions based on a stable distribution.
‌⁠⁠Linux Mint was started as a fork of Ubuntu Linux, while still relying upon the Ubuntu repositories. There are various versions, all free of cost, but some include proprietary codecs, which cannot be distributed without license restrictions in certain countries.
Android

```text
Linux is a kernel, and many of the commands covered in this course are actually part of the GNU package. That is why some people insist on using the term GNU/Linux instead of Linux alone.
```

Android, sponsored by Google, is the world’s most popular Linux distribution. It is fundamentally different from its counterparts. Android uses the Dalvik virtual machine with Linux, providing a robust platform for mobile devices such as phones and tablets. However, lacking the traditional packages that are often distributed with Linux (such as GNU and Xorg), Android is generally incompatible with desktop Linux distributions.
This incompatibility means that a Red Hat or Ubuntu user cannot download software from the Google Play store. Likewise, a terminal emulator in Android lacks many of the commands of its Linux counterparts. It is possible, however, to use BusyBox with Android to enable most commands to work.
Other
Raspbian is a specialized Linux distribution optimized to run on Raspberry Pi hardware. This combination has seen significant use in training for programmers and hardware designers at all levels. Its low cost and ease of use have made it a favorite of educators worldwide, and many add-on devices are available to extend its capabilities into the physical world. There is a multitude of labs and projects available that teach everything from environmental monitoring to circuit design, machine learning, and robotics.

```text
Linux From Scratch (LFS) is more of a learning tool than a working distribution. This project consists of an online book, and source code, with “step-by-step instructions” for building a custom Linux distribution from the source code up. This “distribution” embodies the true spirit of Linux whereby users can modify any aspect of the operating system and learn how all the pieces work together. It’s also a good starting point for anyone who needs specialized functionality or an ultra-compact build for an embedded system project.
```

We have discussed the distributions explicitly mentioned in the Linux Essentials objectives. Be aware that there are hundreds, if not thousands more that are available. While there are many different distributions of Linux, many of the programs and commands remain the same or are very similar.

#### 2.4.2 Embedded Systems

```text
Linux started out as something that would only run on a computer like Linus Torvald's: an Intel 386 PC with a specific hard drive controller, but since anyone could add to or change Linux, people started building support for other hardware. Eventually, Linux started supporting other chips with an emphasis on small size and low power consumption.
```

Because of this flexibility, a significant number of device makers have used Linux as the operating system for their hardware products. Today we call these embedded systems because they are designed to do a specific task on hardware optimized for only that purpose. These systems encompass a tremendous diversity of devices that are used today, from cell phones to smart TVs and appliances, to remote monitoring systems for pipelines and factories.
As Linux evolved, specialized processor chips were developed for consumer and industrial devices to take advantage of its capabilities. Support for Linux has become so ubiquitous that it is possible to prototype and bring to market new devices using off-the-shelf components. The rise of cheap, small, adaptable single-board computers like the Raspberry Pi has given experimenters and entrepreneurs everywhere tools to quickly build custom solutions, powered by Linux, that would have taken months of work by specialized teams just a few years ago.
While consumers are familiar with embedded Linux entertainment devices like digital video recorders (DVRs) and “smart TVs,” the real impact of embedded Linux is just starting to be realized. The internet of things (IoT) is just ramping up with cheap, ubiquitous devices being deployed on everything from oil wells to solar generating farms. These networks of smart sensors and controllers enable engineers to adjust critical processes in real time while monitoring and reporting back to central control stations. As more processes are being monitored and more data is being integrated with machine learning and artificial intelligence (AI) we can anticipate gains in efficiency, safety and productivity only dreamed of by past generations.

### 3.1 Navigating the Linux Desktop

To be a Linux systems administrator, it is necessary to be comfortable with Linux as a desktop operating system and have proficiency with basic Information and Communication Technology (ICT) skills. Using Linux for productivity tasks, rather than depending on Windows or Macintosh systems, accelerates learning by working with Linux tools on a daily basis. Systems administrators do far more than manage servers; they are often called upon to assist users with configuration issues, recommend new software, and update documentation among other tasks.
Most Linux distributions allow users to download a “desktop” installation package that can be loaded onto a USB key. This is one of the first things aspiring system administrators should do; download a major distribution and load it onto an old PC. This process is fairly straightforward, and tutorials are available online. The Linux desktop should be familiar to anyone who has used a PC or Macintosh with icons to select different programs and a “settings” application to configure things like user accounts, WiFi networks, and input devices. After familiarizing oneself with the Linux Graphical User Interface (GUI), or desktop, the next step is learning how to perform tasks from the command line.

#### 3.1.1 Getting to the Command Line

The command line interface (CLI) is a simple text input system for entering anything from single-word commands to complicated scripts. Most operating systems have a CLI that provides a direct way of accessing and controlling the computer.
On systems that boot to a GUI, there are two common ways of accessing the command line—a GUI-based terminal, and a virtual terminal:
- A GUI terminal is a program within the GUI environment that emulates a terminal window. GUI terminals can be accessed through the menu system. For example, on a CentOS machine, you could click on Applications on the menu bar, then System Tools > and, finally, Terminal. If you have a search tools, you can search for terminal, as shown here.

- A virtual terminal can be run at the same time as a GUI but requires the user to log in via the virtual terminal before they can execute commands (as they would before accessing the GUI interface).
Each Linux desktop distribution is slightly different, but the application terminal or x-term will open a terminal window from the GUI. While there are subtle differences between the terms console and terminal window sessions, they are all the same from an administrators standpoint and require the same knowledge of commands to use.
Ordinary command line tasks are starting programs, parsing scripts, and editing text files used for system or application configuration. Most servers boot directly to a terminal, as a GUI can be resource intensive and is generally not needed to perform server-based operations.‌⁠​​

### 3.2 Applications

The kernel of the operating system is like an air traffic controller at an airport, and the applications are the airplanes under its control. The kernel decides which program gets which blocks of memory, it starts and kills applications, and it handles displaying text or graphics on a monitor.
Applications make requests to the kernel and in return receive resources, such as memory, CPU, and disk space. If two applications request the same resource, the kernel decides which one gets it, and in some cases, kills off another application to save the rest of the system and prevent a crash.
The kernel also abstracts some complicated details away from the application. For example, the application doesn’t know if a block of disk storage is on a solid-state drive, a spinning metal hard disk, or even a network file share. Applications need only follow the kernel’s Application Programming Interface (API) and therefore don’t have to worry about the implementation details. Each application behaves as if it has a large block of memory on the system; the kernel maintains this illusion by remapping smaller blocks of memory, sharing blocks of memory with other applications, or even swapping out untouched blocks to disk.
The kernel also handles the switching of applications, a process known as multitasking. A computer system has a small number of central processing units (CPUs) and a finite amount of memory. The kernel takes care of unloading one task and loading a new one if there is more demand than resources available. When one task has run for a specified amount of time, the CPU pauses it so that another may run. If the computer is doing several tasks at once, the kernel is deciding when to switch focus between tasks. With the tasks rapidly switching, it appears that the computer is doing many things at once.
When we, as users, think of applications, we tend to think of word processors, web browsers, and email clients, however, there are a large variety of application types. The kernel doesn’t differentiate between a user-facing application, a network service that talks to a remote computer, or an internal task. From this, we get an abstraction called a process. A process is just one task that is loaded and tracked by the kernel. An application may even need multiple processes to function, so the kernel takes care of running the processes, starting and stopping them as requested, and handing out system resources.

### 5.1 Introduction

Most consumer operating systems are designed to shield the user from the ins and outs of the CLI. The Linux community is different in that it positively celebrates the CLI for its power, speed and ability to accomplish a vast array of tasks with a single command line instruction.
When a user first encounters the CLI, they can find it challenging because it requires memorizing a dizzying amount of commands and their options. However, once a user has learned the structure of how commands are used, where the necessary files and directories are located and how to navigate the hierarchy of a file system, they can be immensely productive. This capability provides more precise control, greater speed and the ability to automate tasks more easily through scripting.
Furthermore, by learning the CLI, a user can easily be productive almost instantly on ANY flavor or distribution of Linux, reducing the amount of time needed to familiarize themselves with a system because of variations in a GUI.

### 5.2 Shell

Once a user has entered a command the terminal then accepts what the user has typed and passes it to a shell. The shell is the command line interpreter that translates commands entered by a user into actions to be performed by the operating system. If output is produced by the command, then text is displayed in the terminal. If problems with the command are encountered, an error message is displayed.
The Linux environment allows the use of many different shells, some of which have been around for many years. The most commonly-used shell for Linux distributions is called the Bash shell. Bash provides many advanced features, such as command history and inline editing, which allows a user to easily re-execute previously executed commands or a variation of them via simple editing.
The Bash shell also has other popular features, a few of which are listed below:
- Scripting: The ability to place commands in a file and then interpret (effectively use Bash to execute the contents of) the file, resulting in all of the commands being executed. This feature also has some programming features, such as conditional statements and the ability to create functions (AKA subroutines).
- Aliases: The ability to create short nicknames for longer commands.
- Variables: Used to store information for the Bash shell and for the user. These variables can be used to modify how commands and features work as well as provide vital system information.
Bash has an extensive feature list; this is only a sampling of its capabilities.
When a terminal application is run, and a shell appears, displaying an important part of the interface—the prompt. Not only is the prompt there to indicate that commands can be run, but it also conveys useful information to the user. The prompt is fully configurable and can be as sparse or as full-featured as is practical and useful.
The structure of the prompt may vary between distributions, but typically contains information about the user and the system. Below is a common prompt structure:

```text
sysadmin@localhost:~$
```

The prompt shown contains the following information:
1. User Name:

```text
sysadmin@localhost:~$
2. System Name:
sysadmin@localhost:~$
3. Current Directory:
sysadmin@localhost:~$
```

The ~ symbol is used as shorthand for the user's home directory. Typically the home directory for the user is under the /home directory and named after the user account name; for example, /home/sysadmin.

### 5.4 Variables

A variable is a feature that allows the user or the shell to store data. This data can be used to provide critical system information or to change the behavior of how the Bash shell (or other commands) work. Variables are given names and stored temporarily in memory. There are two types of variables used in the Bash shell: local and environment.

#### 5.4.1 Local Variables

Local or shell variables exist only in the current shell, and cannot affect other commands or applications. When the user closes a terminal window or shell, all of the variables are lost. They are often associated with user-based tasks and are lowercase by convention.
To set the value of a variable, use the following assignment expression. If the variable already exists, the value of the variable is modified. If the variable name does not already exist, the shell creates a new local variable and sets the value:

```text
variable=value
```

The following example creates a local variable named variable1 and assigns it a value of Something:

```text
sysadmin@localhost:~$ variable1='Something'
```

The echo command is used to display output in the terminal. To display the value of the variable, use a dollar sign $ character followed by the variable name as an argument to the echo command:

```text
sysadmin@localhost:~$ echo $variable1
Something

#### 5.4.2 Environment Variables

```

Environment variables, also called global variables, are available system-wide, in all shells used by Bash when interpreting commands and performing tasks. The system automatically recreates environment variables when a new shell is opened. Examples include the PATH, HOME, and HISTSIZE variables. The HISTSIZE variable defines how many previous commands to store in the history list. The command in the example below displays the value of the HISTSIZE variable:

```text
sysadmin@localhost:~$ echo $HISTSIZE
```

1000
To modify the value of an existing variable, use the assignment expression:

```text
sysadmin@localhost:~$ HISTSIZE=500
sysadmin@localhost:~$ echo $HISTSIZE
```

500
Many variables are available for the Bash shell, as well as variables that affect different Linux commands. A discussion of all variables is beyond the scope of this chapter; however, more shell variables will be covered as this course progresses.
When run without arguments, the env command outputs a list of the environment variables. Because the output of the env command can be quite long, the following examples use a text search to filter that output.
In a previous example variable1 was created as a local variable, so the following search in the environment variables results in no output:

```text
sysadmin@localhost:~$ env | grep variable1
```

The pipe | character passes the output of the env command to the grep command, which searches the output.
This text filtering technique will be covered in detail later in the course.
The export command is used to turn a local variable into an environment variable.
export variable
After exporting variable1, it is now an environment variable. It is now found in the search through the environment variables:

```text
sysadmin@localhost:~$ export variable1
sysadmin@localhost:~$ env | grep variable1
variable1=Something
```

The export command can also be used to make a variable an environment variable upon its creation by using the assignment expression as the argument:

```text
sysadmin@localhost:~$ export variable2='Else'
sysadmin@localhost:~$ env | grep variable2
variable2=Else
```

To change the value of an environment variable, use the assignment expression:

```text
sysadmin@localhost:~$ variable1=$variable1' '$variable2
sysadmin@localhost:~$ echo $variable1
Something Else
```

Exported variables can be removed using the unset command:

```text
sysadmin@localhost:~$ unset variable2

#### 5.4.3 Path Variable

```

One of the most important Bash shell variables to understand is the PATH variable. It contains a list that defines which directories the shell looks in to find commands. If a valid command is entered and the shell returns a "command not found" error, it is because the Bash shell was unable to locate a command by that name in any of the directories included in the path. The following command displays the path of the current shell:

```text
sysadmin@localhost:~$ echo $PATH
```

/home/sysadmin/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games

```text
sysadmin@localhost:~$
```

Each directory in the list is separated by a colon : character. Based on the preceding output, the path contains the following directories. The shell will check the directories in the order they are listed:
/home/sysadmin/bin
/usr/local/sbin
/usr/local/bin
/usr/sbin
/usr/bin
/sbin
/bin
/usr/games
Each of these directories is represented by a path. A path is a list of directories separated by the / character. If you think of the filesystem as a map, paths are the directory addresses, which include step-by-step navigation directions; they can be used to indicate the location of any file within the filesystem. For example, /home/sysadmin is a path to the home directory:

Directories and paths will be covered in detail later in the course.
If the command is not found in any directory listed in the PATH variable, then the shell returns an error:

```text
sysadmin@localhost:~$ zed
```

-bash: zed: command not found

```text
sysadmin@localhost:~$
```

‌⁠​​⁠​ If custom software is installed on the system it may be necessary to modify the PATH to make it easier to execute these commands. For example, the following will add and verify the /usr/bin/custom directory to the PATH variable:

```text
sysadmin@localhost:~$ PATH=/usr/bin/custom:$PATH
sysadmin@localhost:~$ echo $PATH
```

/usr/bin/custom:/home/sysadmin/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games
When updating the PATH variable, always include the current path, so as not to lose access to commands located in those directories. This can be accomplished by appending $PATH to the value in the assignment expression. Recall that a variable name preceded by a dollar sign represents the value of the variable.

### 5.5 Command Types

One way to learn more about a command is to look at where it comes from. The type command can be used to determine information about command type.
type command
There are several different sources of commands within the shell of your CLI including internal commands, external commands, aliases, and functions.

#### 5.5.2 External Commands

External commands are binary executables stored in directories that are searched by the shell. If a user types the ls command, then the shell searches through the directories that are listed in the PATH variable to try to find a file named ls that it can execute.
If a command does not behave as expected or if a command is not accessible that should be, it can be beneficial to know where the shell is finding the command or which version it is using. It would be tedious to have to manually look in each directory that is listed in the PATH variable. Instead, use the which command to display the full path to the command in question:
which command
The which command searches for the location of a command by searching the PATH variable.

```text
sysadmin@localhost:~$ which ls
```

/bin/ls

```text
sysadmin@localhost:~$ which cal
```

/usr/bin/cal
External commands can also be executed by typing the complete path to the command. For example, to execute the ls command:

```text
sysadmin@localhost:~$ /bin/ls
Desktop  Documents  Downloads  Music  Pictures  Public  Templates  Videos
```

For external commands, the type command displays the location of the command:

```text
sysadmin@localhost:~$ type cal
cal is /usr/bin/cal
```

In some cases the output of the type command may differ significantly from the output of the which command:

```text
sysadmin@localhost:~$ type echo
echo is a shell builtin
sysadmin@localhost:~$ which echo
```

/bin/echo
Using the -a option of the type command displays all locations that contain the command named:

```text
sysadmin@localhost:~$ type -a echo
echo is a shell builtin
echo is /bin/echo

#### 5.5.3 Aliases

```

An alias can be used to map longer commands to shorter key sequences. When the shell sees an alias being executed, it substitutes the longer sequence before proceeding to interpret commands.
For example, the command ls -l is commonly aliased to l or ll. Because these smaller commands are easier to type, it becomes faster to run the ls -l command line.
To determine what aliases are set on the current shell use the alias command:

```text
sysadmin@localhost:~$ alias
alias egrep='egrep --color=auto'
alias fgrep='fgrep --color=auto'
alias grep='grep --color=auto'
alias l='ls -CF'
alias la='ls -A'
alias ll='ls -alF'
alias ls='ls --color=auto'
```

The aliases from the previous examples were created by initialization files. These files are designed to make the process of creating aliases automatic.
New aliases can be created using the following format, where name is the name to be given the alias and command is the command to be executed when the alias is run.

```text
alias name=command
```

For example, the cal 2019 command displays the calendar for the year 2019. Suppose you end up running this command often. Instead of executing the full command each time, you can create an alias called mycal and run the alias, as demonstrated in the following graphic:

```text
sysadmin@localhost:~$ alias mycal="cal 2019"
sysadmin@localhost:~$ mycal
```

2019
January               February               March
Su Mo Tu We Th Fr Sa  Su Mo Tu We Th Fr Sa  Su Mo Tu We Th Fr Sa

## 1 2 3 4 5 1 2 1 2

## 6 7 8 9 10 11 12 3 4 5 6 7 8 9 3 4 5 6 7 8 9

## 13 14 15 16 17 18 19 10 11 12 13 14 15 16 10 11 12 13 14 15 16

## 20 21 22 23 24 25 26 17 18 19 20 21 22 23 17 18 19 20 21 22 23

## 27 28 29 30 31 24 25 26 27 28 24 25 26 27 28 29 30

31
Aliases created this way only persist while the shell is open. Once the shell is closed, the new aliases are lost. Additionally, each shell has its own aliases, so aliases created in one shell won’t be available in a new shell that’s opened.
The type command can identify aliases to other commands:

```text
sysadmin@localhost:~$ type ll
```

ll is aliased to `ls -alF'

```text
sysadmin@localhost:~$ type -a ls
```

ls is aliased to `ls --color=auto'

```text
ls is /bin/ls
```

The output of these commands indicates that ll is an alias for ls -alF, and even ls is an alias for ls --color=auto.

#### 5.5.4 Functions

Functions can also be built using existing commands to either create new commands, or to override commands built-in to the shell or commands stored in files. Aliases and functions are normally loaded from the initialization files when the shell first starts.
Functions are more advanced than aliases and typically are used in Bash shell scripts. Typically, functions are used to execute multiple commands. To create a function, the following syntax is used:
function_name ()
{
commands
}
In the format above, function_name can be anything that the administrator wants to call the function. The commands that the administrator wants to execute can replace the commands placeholder. Note the formatting, in particular, the location of the parenthesis () and braces {}, as well as the convention of using tabs to make the function more easily readable.
Functions are useful as they allow for a set of commands to be executed one at a time instead of typing each command repeatedly. In the example below, a function called my_report is created to execute the ls, date, and echo commands.

```text
sysadmin@localhost:~$ my_report () {
> ls Documents
> date
> echo "Document directory report"
> }
```

When creating a function, a > character will appear as a prompt to enter the commands for the function. The curly braces {} are used to let the shell know when a function begins and ends so as to exit the > prompt.
Once a function is created, the function name may be invoked from the BASH prompt to execute the function:

```text
sysadmin@localhost:~$ my_report
```

School            alpha-third.txt  hidden.txt    numbers.txt  spelling.txt
Work              alpha.txt        letters.txt   os.csv       words
adjectives.txt    animals.txt      linux.txt     people.csv
alpha-first.txt   food.txt         longfile.txt  profile.txt
alpha-second.txt  hello.sh         newhome.txt   red.txt
Wed Oct 13 06:54:04 UTC 2021
Document directory report

```text
sysadmin@localhost:~$

### 5.6 Quoting

```

Quotation marks are used throughout Linux administration and most computer programming languages to let the system know that the information contained within the quotation marks should either be ignored or treated in a way that is very different than it would normally be treated. There are three types of quotes that have special significance to the Bash shell: double quotes ", single quotes ', and back quotes `. Each set of quotes alerts the shell not to treat the text within the quotes in the normal way.

#### 5.6.1 Double Quotes

Double quotes stop the shell from interpreting some metacharacters (special characters), including glob characters.
Glob characters, also called wild cards, are symbols that have special meaning to the shell; they are interpreted by the shell itself before it attempts to run any command. Glob characters include the asterisk * character, the question ? mark character, and the brackets [ ], among others.
Globbing will be covered in greater detail later in the course.
Within double quotes an asterisk is just an asterisk, a question mark is just a question mark, and so on, which is useful when you want to display something on the screen that is normally a special character to the shell. In the echo command below, the Bash shell doesn't convert the glob pattern into filenames that match the pattern:

```text
sysadmin@localhost:~$ echo "The glob characters are *, ? and [ ]"
```

The glob characters are *, ? and [ ]
Double quotes still allow for command substitution, variable substitution, and permit some other shell metacharacters that haven't been discussed yet. The following demonstration shows that the value of the PATH variable is still displayed:

```text
sysadmin@localhost:~$ echo "The path is $PATH"
The path is /usr/bin/custom:/home/sysadmin/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games

#### 5.6.2 Single Quotes

```

Single quotes prevent the shell from doing any interpreting of special characters, including globs, variables, command substitution and other metacharacters that have not been discussed yet.
For example, to make the $ character simply mean a $, rather than it acting as an indicator to the shell to look for the value of a variable, execute the second command displayed below:

```text
sysadmin@localhost:~$ echo The car costs $100
```

The car costs 00

```text
sysadmin@localhost:~$ echo 'The car costs $100'
```

The car costs $100

#### 5.6.3 Backslash Character

There is also an alternative technique to essentially single quote a single character. Consider the following message:

```text
The service costs $1 and the path is $PATH
```

If this sentence is placed in double quotes, $1 and $PATH are considered variables.

```text
sysadmin@localhost:~$ echo "The service costs $1 and the path is $PATH"

```

‌⁠​​⁠​The service costs  and the path is /usr/bin/custom:/home/sysadmin/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games
If it is placed in single quotes, $1 and $PATH are not considered variables.

```text
sysadmin@localhost:~$ echo 'The service costs $1 and the path is $PATH'
The service costs $1 and the path is $PATH
```

But what if you want to have $PATH treated as a variable and $1 not?
In this case, use a backslash \ character in front of the dollar sign $ character to prevent the shell from interpreting it. The command below demonstrates using the \ character:

```text
sysadmin@localhost:~$ echo The service costs \$1 and the path is $PATH
The service costs $1 and the path is /usr/bin/custom:/home/sysadmin/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games

#### 5.6.4 Backquotes

```

Backquotes, or backticks, are used to specify a command within a command, a process called command substitution. This allows for powerful and sophisticated use of commands.
While it may sound confusing, an example should make things more clear. To begin, note the output of the date command:

```text
sysadmin@localhost:~$ date
```

Mon Nov  4 03:35:50 UTC 2018
Now, note the output of the echo command:

```text
sysadmin@localhost:~$ echo Today is date
```

Today is date
In the previous command, the word date is treated as regular text, and the shell passes date to the echo command. To execute the date command and have the output of that command sent to the echo command, put the date command in between two backquote characters:

```text
sysadmin@localhost:~$ echo Today is `date`
```

Today is Mon Nov 4 03:40:04 UTC 2018

### 5.7 Control Statements

Control statements allow you to use multiple commands at once or run additional commands, depending on the success of a previous command. Typically these control statements are used within scripts, but they can also be used on the command line as well.

#### 5.7.1 Semicolon

command1; command2; command3
The semicolon ; character can be used to run multiple commands, one after the other. Each command runs independently and consecutively; regardless of the result of the first command, the second command runs once the first has completed, then the third and so on.
For example, to print the months of January, February and March of 2030, execute the following command:

```text
sysadmin@localhost:~$ cal 1 2030; cal 2 2030; cal 3 2030
```

January 2030
Su Mo Tu We Th Fr Sa

## 1 2 3 4 5

## 6 7 8 9 10 11 12

## 13 14 15 16 17 18 19

## 20 21 22 23 24 25 26

## 27 28 29 30 31

February 2030
Su Mo Tu We Th Fr Sa

## 1 2

## 3 4 5 6 7 8 9

## 10 11 12 13 14 15 16

## 17 18 19 20 21 22 23

## 24 25 26 27 28

March 2030
Su Mo Tu We Th Fr Sa

## 1 2

## 3 4 5 6 7 8 9

## 10 11 12 13 14 15 16

## 17 18 19 20 21 22 23

## 24 25 26 27 28 29 30

31

#### 5.7.2 Double Ampersand

command1 && command2
The double ampersand && acts as a logical "and"; if the first command is successful, then the second command will also run. If the first command fails, then the second command will not run.
To better understand how this works, consider first the concept of failure and success for commands. Commands succeed when they work properly and fail when something goes wrong. For example, consider the ls command. The command succeeds if the given directory is accessible and fails if it isn't.
In the following example, the first command succeeds because the /etc/ppp directory exists and is accessible while the second command fails because there is no /junk directory:

```text
sysadmin@localhost:~$ ls /etc/ppp
ip-down.d  ip-up.d
sysadmin@localhost:~$ ls /etc/junk
```

ls: cannot access /etc/junk: No such file or directory
To use the success or failure of the ls command in conjunction with && execute commands like the following. In the first example, the echo command is executed because the ls command succeeds:

```text
sysadmin@localhost:~$ ls /etc/ppp && echo success
ip-down.d  ip-up.d
```

success
In the second example, the echo command isn't executed because the ls command fails:

```text
sysadmin@localhost:~$ ls /etc/junk && echo success
```

ls: cannot access /etc/junk: No such file or directory

#### 5.7.3 Double Pipe

command1 || command2
The double pipe || is a logical "or". Depending on the result of the first command, the second command will either run or be skipped.
With the double pipe, if the first command runs successfully, the second command is skipped; if the first command fails, then the second command is run. In other words, you are essentially telling the shell, "Either run this first command or the second one”.
In the following example, the echo command only executes if the ls command fails:

```text
sysadmin@localhost:~$ ls /etc/ppp || echo failed
ip-down.d  ip-up.d
sysadmin@localhost:~$ ls /etc/junk || echo failed
```

ls: cannot access /etc/junk: No such file or directory
failed

### 4.1 Introduction

Software projects take the form of source code, which is a human-readable set of computer instructions. Since source code is not understood directly by the computer, it must be compiled into machine instructions by a compiler. The compiler is a special program that gathers all of the source code files and generates instructions that can be run on the computer, such as by the Linux kernel.
Historically, commercial software has been sold under a closed source license, meaning that users have the right to use the machine code, also known as the binary or executable, but cannot see the source code. Often the license explicitly states that users may not attempt to reverse engineer the machine code back to source code to figure out what it does.

> **Consider This**
>
Source code compiled into binary programs is one method of creating programs and running computing instructions. Another is the many types of interpreted languages, such as PERL, Python and even BASH scripting, where the code is not compiled, but fed to an interpreting program, typically a binary executable that understands and implements the instructions contained in the source code or scripts.
The development of Linux closely parallels the rise of open source software. Early on there was shareware, freely available programs where users did not necessarily have access to the source code. There were a lot of good things about this, but it was also problematic because malicious programs could be disguised as innocent-looking games, screensavers, and utilities.
Open source takes a source-centric view of software. The open source philosophy is that users have the right to obtain the software source code, and to expand and modify programs for their own use. This also meant the code could be inspected for backdoors, viruses, and spyware. By creating a community of developers and users, accountability for bugs, security vulnerabilities, and compatibility issues became a shared responsibility. This new, global community of computer enthusiasts was empowered by the growing availability of faster internet services and the world wide web.
There are many different variants of open source, but all agree that users should have access to the source code. Where they differ is in how one can, or must, redistribute changes.

```text
Linux has adopted this philosophy to great success. Since Linux was written in the C programming language, and it mirrored the design and functionality of already established UNIX systems, it naturally became a forum where people could develop and share new ideas. Freed from the constraints of proprietary hardware and software platforms, large numbers of very skilled programmers have been able to contribute to the various distributions, making for software that is often more robust, stable, adaptable, and, frankly, better than the proprietary, closed source offerings which dominated the previous decades.
```

Large organizations were understandably suspicious about using software built in this new way, but over time they realized their best programmers were working on Linux-based open source projects in their spare time. Soon, Linux servers and open source programs began to outperform the expensive, proprietary systems already in place. When it came time to upgrade outdated hardware the same programmers, engineers, and system administrators who had started working on Linux as a hobby were able to convince their bosses to give Linux a try. The rest is, as they say, history.
Before the development of Linux, many corporate and scientific applications ran on proprietary UNIX systems. Companies, universities, and governments that run large server farms liked the stability and relative ease of application development these platforms offered.
UNIX was initially created in 1969. By its fourth edition, in 1973, it had been rewritten in the C programming language that is still prominent today. In 1984 the University of California Berkeley released 4.2BSD which introduced TCP/IP, the networking specification that underpins the Internet. By the early 1990’s, when Linux development started, different companies developing UNIX operating systems realized their systems needed to be compatible, and they started working on the X/Open specification that is still used today.
Over the years, computer scientists and the organizations that employ them have realized the benefit of systems that provide familiar tools and consistent ways of accomplishing specific tasks. The standardization of application programming interfaces (APIs) allows programs written for one specific UNIX or Linux operating system to be ported (converted) relatively easy to run on another. So, while proprietary UNIX systems are still in use throughout the world in environments where "certified" solutions are preferred, the interoperability of these systems alongside Linux computers is valued by industry, academia, and governments that use them.
The importance of standards organizations cannot be overstated. Groups like the IEEE (Institute of Electrical and Electronics Engineers) and POSIX (Portable Operating System Interface), allow professionals from different companies and institutions to collaborate on specifications that make it possible for different operating systems and programs to work together. It doesn’t matter if a program is closed or open source, simple or complex, if it is written to these standards others will be able to use and modify it in the future. Every innovation in computing is built on the work of others who came before. Open source software is a collaboration of different people with different needs and backgrounds all working together to make something better than any one of them could have made individually. Standards are what makes this possible, and the many organizations that create, maintain and promote them are integral to the industry.

### 4.2 Open Source Licensing

When talking about buying software, there are three distinct components:
- Ownership – Who owns the intellectual property behind the software?
- Money Transfer – How does money change hands, if at all?
- Licensing – What do you get? What can you do with the software? Can you use it on only one computer? Can you give it to someone else?
In most cases, the ownership of the software remains with the person or company that created it. Users are only granted a license to use the software; this is a matter of copyright law. The money transfer depends on the business model of the creator. It’s the licensing that differentiates open source software from closed source software.
Two contrasting examples will get things started.
With Microsoft Windows, the Microsoft Corporation owns the intellectual property. The license itself, the End User License Agreement (EULA), is a custom legal document that you must click through, indicating your acceptance, in order to install the software. Microsoft keeps the source code and distributes only binary copies through authorized channels. For most consumer products you are allowed to install the software on one computer and are not allowed to make copies of the disk other than for a backup. You are not allowed to reverse engineer the software. You pay for one copy of the software, which gets you minor updates but not major upgrades.

```text
Linux is owned by Linus Torvalds. He has placed the code under a license called GNU General Public License version 2 (GPLv2). This license, among other things, says that the source code must be made available to anyone who asks and that anyone is allowed to make changes. One caveat to this is that if someone makes changes and distributes them, they must put the changes under the same license so that others can benefit. GPLv2 also says that no one is allowed to charge for distributing the source code other than the actual costs of doing so (such as copying it to removable media).
```

In general, when someone creates something, they also get the right to decide how it is used and distributed. Free and Open Source Software (FOSS) refers to software where this right has been given up; anyone is allowed to view the source code and redistribute it. Linus Torvalds has done that with Linux – even though he created Linux he can’t forbid someone from using it on their computer because he has given up that right through the GPLv2 license.
Software licensing is a political issue, therefore it should come as no surprise that there are many different opinions. Organizations have come up with their own license that embodies their particular views, so it is easier to choose an existing license than come up with your own. For example, universities like the Massachusetts Institute of Technology (MIT) and University of California have come up with licenses, as have projects like the Apache Foundation. Also, groups like the Free Software Foundation have created their own licenses to further their agenda.

#### 4.2.1 The Free Software Foundation

Two groups can be considered the most influential forces in the world of open source: the Free Software Foundation and the Open Source Initiative.
Only a few years after the development of the GNU project, Richard Stallman founded the Free Software Foundation (FSF) in 1985 with the goal of promoting free software. In this context, the word "free" does not refer to the price, but to the freedom to share, study, and modify the underlying source code. According to their website, the FSF believes that users should have "control over the technology we use in our homes, schools, and businesses".
FSF also advocates that software licenses should enforce the openness of modifications. It is their view that if someone modifies free software that they should be required to share any changes they have made when they share it again. This specific philosophy is called copyleft. According to FSF, "copyleft is a general method for making a program (or other work) free (in the sense of freedom, not "zero price"), and requiring all modified and extended versions of the program to be free as well".
The FSF also advocates against software patents and acts as a watchdog for standards organizations, speaking out when a proposed standard might violate the free software principles by including items like Digital Rights Management (DRM) which restrict what can be done with compliant programs.
The FSF have developed their own set of licenses which are free for anyone to use based on the original GNU General Public License (GPL). FSF currently maintains GNU General Public License version 2 (GPLv2) and version 3 (GPLv3), as well as the GNU Lesser General Public Licenses version 2 (LGPLv2) and version 3 (LGPLv3). These licenses are meant to be included in the actual source code to ensure that all future variants and modifications of the original program continue to have the same freedom of use as the original. The GPL license and its variants are powerful legal tools to advance the cause of free software worldwide. What started off in 1983 as one man’s desire to share and improve software by letting others change it has ended up changing the world.

> **Consider This**
>
The changes between GPLv2 and GPLv3 largely focused on using free software on a closed hardware device which has been coined Tivoization. TiVo is a company that builds a television digital video recorder on their own hardware and used Linux as the base for their software. While TiVo released the source code to their version of Linux as required under GPLv2, the hardware would not run any modified binaries. In the eyes of the FSF, this went against the spirit of the GPLv2, so they added a specific clause to version 3 of the license. Linus Torvalds agrees with TiVo on this matter and has chosen to stay with GPLv2.

#### 4.2.2 The ‌⁠​​⁠​ Open Source Initiative

The Open Source Initiative (OSI) was founded in 1998 by Bruce Perens and Eric Raymond. They believed that the Free Software Foundation was too politically charged and that less extreme licenses were necessary, particularly around the copyleft aspects of FSF licenses. OSI believes that not only should the source be freely available, but also that no restrictions should be placed on the use of the software, no matter what the intended use. Unlike the FSF, the OSI does not have its own set of licenses. Instead, the OSI has a set of principles and adds licenses to that list if they meet those principles, called open source licenses. Software that conforms to an Open Source license is, therefore, open source software.
One type of Open Source license is the BSD (Berkeley Software Distribution) and its derivatives, which are much simpler than GPL. There are currently two actual "BSD" licenses approved by OSI, a 2-Clause and a 3-Clause. These licenses state that you may redistribute the source and binaries as long as you maintain copyright notices and don’t imply that the original creator endorses your version. In other words "do what you want with this software, just don’t say you wrote it." According to FSF, the original BSD license had a serious flaw in that it required developers to add a clause acknowledging the University of California, Berkeley in every advertisement for software licensed this way. As others copied this simple license, they included acknowledgment for their own institutions which led to over 75 such acknowledgments in some cases.
FSF licenses, such as GPLv2, are also open source licenses. However, many open source licenses such as BSD and MIT do not contain the copyleft provisions and are thus not acceptable to the FSF. These licenses are called permissive free software licenses because they are permissive in how you can redistribute the software. You can take BSD licensed software and include it in a closed software product as long as you give proper attribution.
Rather than dwell over the finer points of Open Source and Free Software, the community has started referring to them collectively as Free and Open Source Software (FOSS). The English word "free" can mean "free as in lunch" (as in no cost) or "free as in speech" (as in no restrictions). This ambiguity led to the inclusion of the word "libre" to refer to the latter definition. Thus, we end up with Free/Libre/Open Source Software (FLOSS).

#### 4.2.3 Creative Commons

FOSS licenses are mostly related to software. People have placed works such as drawings and plans under FOSS licenses, but this was not the intent.
When software has been placed in the public domain, the author has relinquished all rights, including the copyright on the work. In some countries, this is the default when the work is done by a government agency. In some countries, copyrighted work becomes public domain after the author has died and a lengthy waiting period has elapsed.
The Creative Commons (CC) organization has created the Creative Commons Licenses which try to address the intentions behind FOSS licenses for non-software entities. CC licenses can also be used to restrict commercial use if that is the desire of the copyright holder. The CC licenses are made up of the following set of conditions the creator can apply to their work:
- Attribution (BY) – All CC licenses require that the creator must be given credit, without implying that the creator endorses the use.
- ShareAlike (SA) – This allows others to copy, distribute, perform, and modify the work, provided they do so under the same terms.
- NonCommercial (NC) – This allows others to distribute, display, perform, and modify the work for any purpose other than commercially.
- NoDerivatives (ND) – This allows others to distribute, display, and perform only original copies of the work. They must obtain the creator’s permission to modify it.
These conditions are then combined to create the six main licenses offered by Creative Commons:
- Attribution (CC BY) – Much like the BSD license, you can use CC BY content for any use but must credit the copyright holder.
- Attribution ShareAlike (CC BY-SA) – A copyleft version of the Attribution license. Derived works must be shared under the same license, much like in the Free Software ideals.
- Attribution NoDerivs (CC BY-ND) – You may redistribute the content under the same conditions as CC-BY but may not change it.
- Attribution-NonCommercial (CC BY-NC) – Just like CC BY, but you may not use it for commercial purposes.
- Attribution-NonCommercial-ShareAlike (CC BY-NC-SA) – Builds on the CC BY-NC license but requires that your changes be shared under the same license.
- Attribution-NonCommercial-NoDerivs (CC BY-NC-ND) – You are sharing the content to be used for non-commercial purposes, but people may not change the content.
- No Rights Reserved (CC0) – This is the Creative Commons version of public domain.

### 4.3 Open Source Business Models

If all this software is free, how can anyone make money off of it?
First, you must understand there isn’t anything in the GPL that prohibits selling software. In fact, the right to sell software is part of the GPL license. Again, recall that the word free refers to freedom, not price. Companies that add value to these free programs are encouraged to make as much money as they can, and put those profits back into developing more and better software.
One of the simplest ways to make money is to sell support or warranty around the software. Companies like Canonical, the developer of Ubuntu, and Redhat have grown into huge enterprises by creating Linux distributions and tools that enable commercial users to manage their enterprises and offer products and services to their customers.
Many other open source projects have also expanded into substantial businesses. In the 1990s, Gerald Combs was working at an Internet service provider and started writing his own network analysis tool because similar tools at the time were costly. Over 600 people have now contributed to the project, called Wireshark. It is now often considered better than commercial offerings and led to a company being formed to sell products and support. Like many others, this company was purchased by a larger enterprise that supports its continued development.
Companies like Tivo have packaged hardware or add extra closed source software to sell alongside the free software. Appliances and embedded systems that use Linux are a multi-billion dollar business and encompass everything from home DVRs to security cameras and wearable fitness devices. Many consumer firewalls and entertainment devices follow this model.
Today, both large and small employers have individuals and sometimes whole groups devoted to working on open source projects. Technology companies compete for the opportunity to influence projects that will shape the future of their industries. Other companies dedicate resources towards projects they need for internal use. As more business is done on cloud resources, the opportunity for open source programmers continues to expand.

### 6.1 Introduction

There are thousands of commands available with many options, making the command line a powerful tool. However, with this power comes complexity. Complexity, in turn, can create confusion. As a result, knowing how to find help while working in Linux is an essential skill for any user. Referring to help provides a quick reminder of how a command works, as well as being an information resource when learning new commands.

### 6.2 Man Pages

UNIX is the operating system that Linux was modeled after. The developers of UNIX created help documents called man pages (short for manual pages).
Man pages are used to describe the features of commands. They provide a basic description of the purpose of the command, as well as details regarding available options.

#### 6.2.1 Viewing Man Pages

To view a man page for a command, use the man command:
man command
For example, the following displays the man page for the ls command:

```text
sysadmin@localhost:~$ man ls
```

Navigate the document using the arrow keys:
LS(1)                            User Commands                           LS(1)

NAME
ls - list directory contents

SYNOPSIS
ls [OPTION]... [FILE]...

DESCRIPTION
List  information  about  the FILEs (the current directory by default).
Sort entries alphabetically if none of -cftuvSUX nor --sort  is  speci-
fied.

Mandatory  arguments  to  long  options are mandatory for short options
too.

-a, --all
do not ignore entries starting with .
To exit viewing a man page, use the Q key.

> **Consider This**
>
The man command uses a pager to display documents. Usually, this pager is the less command, but on some distributions, it may be the more command. Both are very similar in how they perform.
To view the various movement commands that are available, use the H key while viewing a man page. This displays a help page.
Pagers will be discussed in more detail later in the course.

#### 6.2.2 Sections Within Man Pages

Man pages are broken into sections. Each section is designed to provide specific information about a command. While there are common sections seen in most man pages, some developers also create sections only available on specific man pages.
The following describes some of the more common sections found in man pages:
NAME
Provides the name of the command and a very brief description.
NAME
ls - list directory contents
SYNOPSIS
Provides examples of how the command is executed.
SYNOPSIS
ls [OPTION]... [FILE]...
The SYNOPSIS section of a man page can be difficult to understand but is very important because it provides a concise example of how to use the command. For example, consider the SYNOPSIS of the man page for the cal command:
SYNOPSIS
cal [-31jy] [-A number] [-B number] [-d yyyy-mm] [[month] year]
The square brackets [ ] are used to indicate that this feature is not required to run the command. For example, [-31jy] means options -3, -1, -j, or -y are available, but not required for the cal command to function properly.
The last set of square brackets [[month] year] demonstrates another feature; it means a year can be specified by itself, but to specify a month the year must also be specified.
Another component of the SYNOPSIS that might cause some confusion can be seen in the man page of the date command:
SYNOPSIS
date [OPTION]... [+FORMAT]
date [-u|--utc|--universal] [MMDDhhmm[[CC]YY][.ss]]
In this SYNOPSIS there are two syntaxes for the date command. The first one is used to display the date on the system while the second is used to set the date.
The ellipsis ... following [OPTION] indicates that one or more of the items before it may be used.
Additionally, the [-u|--utc|--universal] notation means that either the -u option or the --utc option or the --universal option may be used. Typically this means that all three options really do the same thing, but sometimes the use of the | character is used to indicate that the options can't be used in combination, like a logical “or".
DESCRIPTION
Provides a more detailed description of the command.
DESCRIPTION
List  information  about  the FILEs (the current directory by default).
Sort entries alphabetically if none of -cftuvSUX nor --sort  is  speci-
fied.
OPTIONS
Lists the options for the command as well as a description of how they are used. Often this information is found in the DESCRIPTION section and not in a separate OPTIONS section.
-a, --all
do not ignore entries starting with .

-A, --almost-all
do not list implied . and ..

--author
with -l, print the author of each file

-b, --escape
print C-style escapes for nongraphic characters

--block-size=SIZE
scale sizes by SIZE before printing them; e.g., '--block-size=M'
prints sizes in units of 1,048,576 bytes; see SIZE format below
FILES
Lists the files that are associated with the command as well as a description of how they are used. These files may be used to configure the command's more advanced features. Often this information is found in the DESCRIPTION section and not in a separate FILES section.
AUTHOR
Provides the name of the person who created the man page and (sometimes) how to contact the person.
AUTHOR
Written by Richard M. Stallman and David MacKenzie.
REPORTING BUGS
Provides details on how to report problems with the command.
REPORTING BUGS
GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Report ls translation bugs to <http://translationproject.org/team/>
COPYRIGHT
Provides basic copyright information.
COPYRIGHT
Copyright (C) 2017 Free Software Foundation, Inc.  License GPLv3+:  GNU
GPL version 3 or later <http://gnu.org/licenses/gpl.html>.
This  is  free  software:  you  are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law.
SEE ALSO
Provides you with an idea of where you can find additional information. This often includes other commands that are related to this command.
SEE ALSO
Full documentation at: <http://www.gnu.org/software/coreutils/ls>
or available locally via: info '(coreutils) ls invocation'

#### 6.2.4 Man Pages Categorized by Sections

Until now, we have been displaying man pages for commands. However, there are several different types of commands (user commands, system commands, and administration commands), configuration files and other features, such as libraries and kernel components, that require documentation.
As a result, there are thousands of man pages on a typical Linux distribution. To organize all of these man pages, they are categorized by sections.
By default, there are nine sections of man pages:
1. General Commands
2. System Calls
3. Library Calls
4. Special Files
5. File Formats and Conventions
6. Games
7. Miscellaneous
8. System Administration Commands
9. Kernel Routines
The man command searches each of these sections in order until it finds the first match. For example, if you execute the command man cal, the first section (General Commands) is searched for a man page called cal. If not found, then the second section is searched. If no man page is found after searching all sections, an error message is returned:

```text
sysadmin@localhost:~$ man zed
```

No manual entry for zed
To determine which section a specific man page belongs to, look at the numeric value on the first line of the output of the man page. For example, the cal command belongs to the first section of man pages:
CAL(1)                    BSD General Commands Manual             CAL(1)
Sometimes there are man pages with the same name in different sections. In these cases, it may be necessary to specify the section of the correct man page.
For example, there is a command called passwd that allows you to change your password. There is also a file called passwd that stores account information. Both the command and the file have a man page.
The passwd command is a user command, so the associated man page is in the first section. The man command displays the man page for the passwd command by default:

```text
sysadmin@localhost:~$ man passwd
```

PASSWD(1)                        User Commands                 PASSWD(1)
So how do you display the man page for the passwd file? First, determine in which section the man page is located. To search for man pages by name, use the -f option to the man command. It displays man pages that match, or partially match, a specific name and provide the section number and a brief description of each man page:

```text
sysadmin@localhost:~$ man -f passwd
```

passwd (5)           - the password file
passwd (1)           - change user password
passwd (1ssl)        - compute password hashes
Note: On most Linux distributions, the whatis command does the same thing as man -f. On those distributions, both will produce the same output.
To specify a different section, provide the number of the section as the first argument of the man command. The following command displays the passwd man page located in section 5, which is associated with the passwd file:

```text
sysadmin@localhost:~$ man 5 passwd
```

PASSWD(5)                File Formats and Conversions          PASSWD(5)
Unfortunately, you won't always remember the exact name of the man page that you want to view. Fortunately, each man page has a short description associated with it. The -k option to the man command searches both the names and descriptions of the man pages for a keyword.
For example, to find a man page that displays how to copy directories, search for the keyword copy:

```text
sysadmin@localhost:~$ man -k copy
```

cp (1)               - copy files and directories
cpgr (8)             - copy with locking the given file to the password or gr...
cpio (1)             - copy files to and from archives
cppw (8)             - copy with locking the given file to the password or gr...
dd (1)               - convert and copy a file
debconf-copydb (1)   - copy a debconf database
install (1)          - copy files and set attributes
scp (1)              - secure copy (remote file copy program)
ssh-copy-id (1)      - use locally available keys to authorize logins on a re...
Recall that there are thousands of man pages, so when searching for a keyword, be as specific as possible. Using a generic word, such as "the", could result in hundreds or even thousands of results.
Note: On most Linux distributions, the apropos command does the same thing as man -k. On those distributions, both produce the same output.

### 6.3 Finding Commands and Documentation

The whatis command (or man -f) returns what section a man page is stored in. This command occasionally returns unusual output, such as the following:

```text
sysadmin@localhost:~$ whatis ls
```

ls (1)               - list directory contents
ls (lp)              - list directory contents

> **Note**
>
The example above is designed to demonstrate a scenario where two commands list directory contents. The output in the example terminal above may not match the output in the VM.
Based on this output, there are two ls commands that list directory contents. The simple reason for this is that UNIX had two main variants, which resulted in some commands being developed "in parallel" and therefore behaving differently on different variants of UNIX. Many modern distributions of Linux include commands from both UNIX variants.
This does, however, pose a bit of a problem: when the ls command is typed, which command is executed?

### 6.4 Info Documentation

Man pages are excellent sources of information, but they do tend to have a few disadvantages. One example is that each man page is a separate document, not related to any other man page. While some man pages have a SEE ALSO section that may refer to other man pages, they tend to be independent sources of documentation.
The info command also provides documentation on operating system commands and features. The goal is slightly different from man pages: to provide a documentation resource that gives a logical organizational structure, making reading documentation easier.
All of the documentation is merged into a single "book" representing all of the documentation available. Within info documents, information is broken down into categories that work much like a table of contents in a book. Hyperlinks are provided to pages with information on individual topics for a specific command or feature.
Another advantage of info over man pages is that the writing style of info documents is typically more conducive to learning a topic. Consider man pages to be more of a reference resource and info documents to be more of a learning guide.

### 7.1 Introduction

In Linux, everything is considered a file. Files are used to store data such as text, graphics, and programs. Directories are a type of file used to store other files; Windows and Mac OS X users typically refer to them as folders. In any case, directories are used to provide a hierarchical organization structure. However, this structure may be somewhat different depending on the type of system in use.
When working in a Linux operating system, it is important to know how to manipulate files and directories. Some Linux distributions have GUI-based applications that allow you to manage files, but it is advantageous to know how to perform these operations via the command line.

### 7.2 Directory Structure

On a Windows system, the top level of the directory structure is called My Computer. Physical devices, such as hard drives, USB drives, network drives, show up under My Computer and are each assigned a drive letter, such as C: or D:.
The directory structures shown below are provided as examples only. These directories may not be present within the virtual machine environment of this course.
A visual representation of a Windows directory structure:

Like Windows, the Linux directory structure, typically called a filesystem, also has a top level. However instead of My Computer, it is called the root directory, and it is symbolized by the slash / character. Additionally, there are no drives in Linux; each physical device is accessible under a directory, as opposed to a drive letter.
The following image shows a visual representation of a typical Linux filesystem:

To view the contents of the root directory, use the ls command with the / character as the argument:

```text
sysadmin@localhost:~$ ls /
```

bin    etc    lib     mnt    root  'sbin'$'\342\200\214'   tmp
boot   home   lib64   opt    run    srv                    usr
dev    init   media   proc   sbin   sys                    var
Notice that there are many directories with descriptive names including /boot, which contains files to boot the computer.

#### 7.2.1 Home Directory

The term home directory often confuses new Linux users. To begin with, on most Linux distributions there is a directory called home under the root / directory.

Under this /home directory there is a directory for each user on the system. The directory name is the same as the name of the user, so a user named sysadmin would have a home directory called /home/sysadmin.

The home directory is an important directory. To begin with, when a user opens a shell, they should automatically be placed in their home directory, as typically this is where they do most of their work.
Additionally, the home directory is one of the few directories where the user has full control to create and delete additional files and directories. On most Linux distributions, the only users who can access the files in a home directory are the owner and the administrator on the system. Most other directories in a Linux filesystem are protected with file permissions.
File permissions and ownership will be covered in detail later in the course.
The home directory has a special symbol used to represent it; the tilde ~ character. So if the sysadmin user is logged in, the tilde ~ character can be used in place of the /home/sysadmin directory.
It is also possible to refer to another user's home directory by using the tilde ~ character followed by the name of the user account. For example, ~bob would be the equivalent of /home/bob.

#### 7.2.2 Current Directory

To determine where the user is currently located within the filesystem, the pwd (print working directory) command can be used:
pwd [OPTIONS]

```text
sysadmin@localhost:~$ pwd
```

/home/sysadmin
The pwd command prints the working directory, which is the current location of the user within the filesystem. The output of the above command indicates that the sysadmin user is currently in their home directory, shown in the filesystem below:

#### 7.2.3 Changing Directories

When a user opens a shell, they typically begin in their home directory. When you start a fresh virtual machine in our course, either by opening the course or after using the reset button, you are logged in as the sysadmin user, and you begin in the home directory for that user, highlighted in the image below.

To navigate the filesystem, use the cd (change directory) command.
cd [options] [path]
There is a directory called Documents located in the home directory of the sysadmin user. To move from the home directory into the Documents directory use the directory name as an argument to the cd command:

```text
sysadmin@localhost:~$ cd Documents
sysadmin@localhost:~/Documents$

```

When used with no arguments, the cd command will take the user to their home directory.

```text
sysadmin@localhost:~/Documents$ cd
sysadmin@localhost:~$
```

Notice our virtual machines employ a prompt that displays the current working directory, emphasized with the color blue. In the first prompt, the tilde ~ character is equivalent to /home/sysadmin, representing the user's home directory.

```text
sysadmin@localhost:~$
```

After changing directories, the new location ~/Documents can also be confirmed in the new prompt, again shown in blue.

```text
sysadmin@localhost:~$ cd Documents
sysadmin@localhost:~/Documents$

> **Consider This**
>
```

For some commands, no news is good news; there is no output if the cd command is successful. If the user tries to change to a directory that does not exist, the command returns an error message:

```text
sysadmin@localhost:~$ cd Junk
```

-bash: cd: Junk: No such file or directory

### 7.3 Paths

The argument to the cd command is more than just the name of a directory, it is actually a path. A path is a list of directories separated by the / character. If you think of the filesystem as a map, paths are the directory addresses, which include step-by-step navigation directions; they can be used to indicate the location of any file within the filesystem.
For example, /home/sysadmin is a path to the home directory:

There are two types of paths: absolute and relative.

### 7.4 Listing Files in a Directory

For the previous examples, images were provided to show the layout of the filesystem. In practice, maps like these aren’t provided, and users must rely on what’s available in the command line, making the ls (list) command one of the most powerful for navigating the filesystem.
ls [OPTION]... [FILE]...
This ls command is used to display the contents of a directory and can provide detailed information about the files. By default, when it is used with no options or arguments, it lists the files in the current directory:

```text
sysadmin@localhost:~$ ls
Desktop  Documents  Downloads  Music  Pictures  Public  Templates  Videos
```

The ls command can also be used to list the contents of any directory in the filesystem. Provide the path to the directory as an argument:

```text
sysadmin@localhost:~$ ls /var
```

backups  cache  lib  local  lock  log  mail  opt  run  spool  tmp

> **Consider This**
>
On many Linux distributions, including the one used in our virtual machines, the ls command uses color to distinguish by file type. For example, directories may be displayed in blue, executable files may be displayed in green, and symbolic links may be displayed in cyan.
‌⁠​​
Colored output is not the default behavior for the ls command, but rather the effect of the --color option. The ls seems to perform this coloring automatically because there is an alias for the ls command, so it runs with the --color option.

```text
sysadmin@localhost:~$ type ls
```

ls is aliased to `ls --color=auto'
To avoid using the alias, place a backslash character \ in front of your command:

```text
sysadmin@localhost:~$ ls
Desktop  Documents  Downloads  Music  Pictures  Public  Templates  Videos
sysadmin@localhost:~$ \ls
Desktop  Documents  Downloads  Music  Pictures  Public  Templates  Videos

### 8.1 Introduction

```

When working in a Linux Operating System, it is important to know how to manipulate files and directories. Some Linux distributions have GUI-based applications that allow you to manage files, but it is advantageous to know how to perform these operations via the command line.

> **Note**
>
It is important to note that everything in Linux is case-sensitive, a feature carried over from Unix. This means that the shell recognizes a lowercase a-z character as completely different from an uppercase A-Z character. When manipulating files, pay attention to your capitalization: a hello.txt file is different from HELLO.txt and Hello.txt files.
The character standard used for Linux is the UTF-8 standard which is based on the ASCII (American Standard Code for Information Interchange). To learn more about ASCII, execute the man -s 7 ascii command.

### 8.2 Globbing

Glob characters are often referred to as wild cards. These are symbol characters that have special meaning to the shell.
Globs are powerful because they allow you to specify patterns that match filenames in a directory. So instead of manipulating a single file at a time, you can easily execute commands that affect many files. For instance, by using glob characters, it is possible to manipulate all files with a specific extension or with a particular filename length.
Unlike commands that the shell runs, or options and arguments that the shell passes to commands, glob characters are interpreted by the shell itself before it attempts to run any command. As a result, glob characters can be used with any command.
The examples provided in this chapter use the echo command for demonstration.

#### 8.2.1 Asterisk * Character

The asterisk * character is used to represent zero or more of any character in a filename. For example, to display all of the files in the /etc directory that begin with the letter t:

```text
sysadmin@localhost:~$ echo /etc/t*
/etc/terminfo /etc/timezone /etc/tmpfiles.d
```

The pattern t* matches any file in the /etc directory that begins with the character t followed by zero or more of any character. In other words, any files that begin with the letter t.
You can use the asterisk character at any place within the filename pattern. For example, the following matches any filename in the /etc directory that ends with .d:

```text
sysadmin@localhost:~$ echo /etc/*.d
/etc/apparmor.d /etc/binfmt.d /etc/cron.d /etc/depmod.d /etc/init.d /etc/insserv
```

.conf.d /etc/ld.so.conf.d /etc/logrotate.d /etc/modprobe.d /etc/modules-load.d /
etc/pam.d /etc/profile.d /etc/rc0.d /etc/rc1.d /etc/rc2.d /etc/rc3.d /etc/rc4.d

```text
/etc/rc5.d /etc/rc6.d /etc/rcS.d /etc/rsyslog.d /etc/sudoers.d /etc/sysctl.d /et
```

c/tmpfiles.d /etc/update-motd.d
In the next example, all of the files in the /etc directory that begin with the letter r and end with .conf are displayed:

```text
sysadmin@localhost:~$ echo /etc/r*.conf
/etc/resolv.conf /etc/rsyslog.conf

#### 8.2.2 Question Mark ? Character

```

The question mark ? character represents any single character. Each question mark character matches exactly one character, no more and no less.
Suppose you want to display all of the files in the /etc directory that begin with the letter t and have exactly 7 characters after the t character:

```text
sysadmin@localhost:~$ echo /etc/t???????
/etc/terminfo /etc/timezone
```

Glob characters can be used together to find even more complex patterns. The pattern /etc/*???????????????????? command only matches files in the /etc directory with twenty or more characters in the filename:

```text
sysadmin@localhost:~$ echo /etc/*????????????????????
/etc/bindresvport.blacklist /etc/ca-certificates.conf
```

The asterisk and question mark could also be used together to look for files with three-letter extensions by using the /etc/*.??? pattern:

```text
sysadmin@localhost:~$ echo /etc/*.???
/etc/issue.net /etc/locale.gen

#### 8.2.3 Bracket [ ] Characters

```

The bracket [] characters are used to match a single character by representing a range of characters that are possible match characters. For example, the /etc/[gu]* pattern matches any file that begins with either a g or u character and contains zero or more additional characters:

```text
sysadmin@localhost:~$ echo /etc/[gu]*
/etc/gai.conf /etc/groff /etc/group /etc/group- /etc/gshadow /etc/gshadow- /etc/
```

gss /etc/ucf.conf /etc/udev /etc/ufw /etc/update-motd.d /etc/updatedb.conf
Brackets can also be used to a represent a range of characters. For example, the /etc/[a-d]* pattern matches all files that begin with any letter between and including a and d:

```text
sysadmin@localhost:~$ echo /etc/[a-d]*
/etc/adduser.conf /etc/alternatives /etc/apparmor /etc/apparmor.d /etc/apt /etc/
```

bash.bashrc /etc/bind /etc/bindresvport.blacklist /etc/binfmt.d /etc/ca-certific
ates /etc/ca-certificates.conf /etc/calendar /etc/console-setup /etc/cron.d /etc

```text
/cron.daily /etc/cron.hourly /etc/cron.monthly /etc/cron.weekly /etc/crontab /et
```

c/dbus-1 /etc/debconf.conf /etc/debian_version /etc/default /etc/deluser.conf /e
tc/depmod.d /etc/dhcp /etc/dpkg
The /etc/*[0-9]* pattern displays any file that contains at least one number:

```text
sysadmin@localhost:~$ echo /etc/*[0-9]*
/etc/X11 /etc/dbus-1 /etc/iproute2 /etc/mke2fs.conf /etc/python3 /etc/python3.6
/etc/rc0.d /etc/rc1.d /etc/rc2.d /etc/rc3.d /etc/rc4.d /etc/rc5.d /etc/rc6.d
```

The range is based on the ASCII text table. This table defines a list of characters, arranging them in a specific standard order. If an invalid order is provided, no matches will be made:

```text
sysadmin@localhost:~$ echo /etc/*[9-0]*
```

/etc/*[9-0]*

> **Note**
>
The ASCII text table can be viewed in our virtual machines by executing the ascii command.

#### 8.2.4 Exclamation Point ! Character

The exclamation point ! character is used in conjunction with the square brackets to negate a range. For example, the pattern /etc/[!DP]* matches any file that does not begin with a D or P.

```text
sysadmin@localhost:~$ echo /etc/[!a-t]*
/etc/X11 /etc/ucf.conf /etc/udev /etc/ufw /etc/update-motd.d /etc/updatedb.conf
/etc/vim /etc/vtrgb /etc/wgetrc /etc/xdg

#### 8.2.5 Listing With Globs

```

The ls command is normally used to list files in a directory; as a result, using the echo command may seem to have been a strange choice. However, there is something about the ls command that causes problems when listing files using glob patterns.
Keep in mind that it is the shell, not the echo or ls command, that expands the glob pattern into corresponding file names. In other words, if the echo /etc/a* command is executed, what the shell did before executing the echo command was replace a* with all of the files and directories within the /etc directory that match the pattern.
So, if the ls /etc/a* command is run, what the shell would really run would be this:
ls /etc/adduser.conf  /etc/alternatives  /etc/apparmor  /etc/apparmor.d  /etc/apt
When the ls command sees multiple arguments, it performs a list operation on each item separately. In other words, ls /etc/a* is the same as running the following commands consecutively:
ls /etc/adduser.conf
ls /etc/alternatives
ls /etc/apparmor
ls /etc/apparmor.d
ls /etc/apt
Now consider what happens if the ls command is passed a file, such as /etc/adduser.conf:

```text
sysadmin@localhost:~$ ls /etc/adduser.conf
```

/etc/adduser.conf
Running the ls command on a single file results in the name of the file being printed; typically this is useful if the -l option is used to see details about a specific file:

```text
sysadmin@localhost:~$ ls -l /etc/adduser.conf
-rw-r--r-- 1 root root 3028 May 26  2018 /etc/adduser.conf
```

However, what if the ls command is given a directory name as an argument? In this case, the output of the command is different than if the argument was a regular file:

```text
sysadmin@localhost:~$ ls /etc/apparmor
```

init  parser.conf  subdomain.conf
If the ls command is given a directory name, the command displays the contents of the directory (the names of the files in the directory), not just the directory name. The filenames in the previous example are the names of the files in the /etc/apparmor directory.
Why is this a problem when using globs? Consider the following output:

```text
sysadmin@localhost:~$ ls /etc/ap*
```

/etc/apparmor:
init  parser.conf  subdomain.conf

/etc/apparmor.d:
abstractions  disable         local          tunables     usr.sbin.named
cache         force-complain  sbin.dhclient  usr.bin.man  usr.sbin.rsyslogd

/etc/apt:
apt.conf.d  preferences.d  sources.list  sources.list.d  trusted.gpg.d
When the ls command sees a filename as an argument, it just displays the filename. However, for any directory, it displays the contents of the directory, not just the directory name.
This becomes even more confusing in a situation like the following:

```text
sysadmin@localhost:~$ ls /etc/x*
```

autostart  systemd  user-dirs.conf  user-dirs.defaults
In the previous example, it seems like the ls command is just plain wrong. However, what really happened is that the only thing that matches the glob /etc/x* is the /etc/xdg directory.
So, the ls command only displayed the files in that directory!
There is a simple solution to this problem: always use the -d option with globs, which tells the ls command to display the name of directories, instead of their contents:

```text
sysadmin@localhost:~$ls -d /etc/x*
```

/etc/xdg

### 8.3 Copying Files

The cp command is used to copy files. It requires a source and a destination. The structure of the command is as follows:
cp source destination
The source is the file to be copied. The destination is where the copy is to be located. When successful, the cp command does not have any output (no news is good news). The following command copies the /etc/hosts file to your home directory:

```text
sysadmin@localhost:~$ cp /etc/hosts ~
sysadmin@localhost:~$ ls
```

Desktop    Downloads  Pictures  Templates  hosts
Documents  Music      Public    Videos

### 8.4 Moving Files

To move a file, use the mv command. The syntax for the mv command is much like the cp command:
mv source destination
In the following example, the hosts file that was generated previously is moved from the current directory to the Videos directory:

```text
sysadmin@localhost:~$ ls
```

Desktop    Downloads  Pictures  Templates  example.txt  hosts.copy
Documents  Music      Public    Videos     hosts

```text
sysadmin@localhost:~$ mv hosts Videos
sysadmin@localhost:~$ ls
```

Desktop    Downloads  Pictures  Templates  example.txt
Documents  Music      Public    Videos     hosts.copy

```text
sysadmin@localhost:~$ ls Videos
```

hosts
When a file is moved, the file is removed from the original location and placed in a new location. Moving files can be somewhat tricky in Linux because users need specific permissions to remove files from a directory. Without the right permissions, a Permission denied error message is returned:

```text
sysadmin@localhost:~$ mv /etc/hosts .
```

mv: cannot move `/etc/hosts' to `./hosts': Permission denied
Permissions will be covered in detail later in the course.

### 8.5 Creating Files

There are several ways of creating a new file, including using a program designed to edit a file (a text editor).
There is also a way to create an empty file that can be populated with data at a later time. This feature is useful for some operating systems as the very existence of a file could alter how a command or service works. It is also useful to create a file as a "placeholder" to remind you to create the file contents at a later time.
To create an empty file, use the touch command as demonstrated below:

```text
sysadmin@localhost:~$ touch sample
sysadmin@localhost:~$ ls -l sample
-rw-rw-r-- 1 sysadmin sysadmin 0 Nov  9 16:48 sample
```

Notice the size of the new file is 0 bytes. As previously mentioned, the touch command doesn't place any data within the new file.
Text editors will be covered in detail later in the course.

### 8.6 Removing Files

To delete a file, use the rm command:

```text
sysadmin@localhost:~$ ls
```

Desktop    Downloads  Pictures  Templates  hosts.copy
Documents  Music      Public    Videos     sample

```text
sysadmin@localhost:~$ rm sample
sysadmin@localhost:~$ rm hosts.copy
sysadmin@localhost:~$ ls
Desktop  Documents  Downloads  Music  Pictures  Public  Templates  Videos
```

Note that the files were deleted with no questions asked. This could cause problems when deleting multiple files by using glob characters. Because these files are deleted without question, a user could end up deleting files that were not intended to be deleted.
Warning
The files are permanently deleted. There is no command to undelete a file and no trash can from which to recover deleted files.
As a precaution, users should use the -i option when deleting multiple files:

```text
sysadmin@localhost:~$ touch sample.txt example.txt test.txt
sysadmin@localhost:~$ ls
```

Desktop    Downloads  Pictures  Templates  example.txt  test.txt
Documents  Music      Public    Videos     sample.txt

```text
sysadmin@localhost:~$ rm -i *.txt
```

rm: remove regular empty file `example.txt'? y
rm: remove regular empty file `sample.txt'? n
rm: remove regular empty file `test.txt'? y

```text
sysadmin@localhost:~$ ls
```

Desktop    Downloads  Pictures  Templates  sample.txt
Documents  Music      Public    Videos

### 8.7 Creating Directories

To create a directory, use the mkdir command:

```text
sysadmin@localhost:~$ ls
Desktop  Documents  Downloads  Music  Pictures  Public  Templates  sample.txt
sysadmin@localhost:~$ mkdir test
sysadmin@localhost:~$ ls
```

Desktop    Downloads  Pictures  Templates   test
Documents  Music      Public    sample.txt

### 10.1 Introduction

A large number of the files in a typical file system are text files. Text files only contain text, no formatting features that you might see in a word processing file.
Because there are so many of these files on a typical Linux system, a significant number of commands exist to help users manipulate text files. There are commands to both view and modify these files in various ways.
Additionally, there are features available for the shell to control the output of commands, so instead of having the output placed in the terminal window, the output can be redirected into another file or another command. These redirection features provide users with a much more flexible and powerful environment to work within.

#### 10.1.1 Viewing Files in the Terminal

The cat command, short for concatenate, is a simple but useful command whose functions include creating and displaying text files, as well as combining copies of text files. One of the most popular uses of cat is to display the content of text files. To display a file in the standard output using the cat command, type the command followed by the filename:

```text
sysadmin@localhost:~$ cd Documents
sysadmin@localhost:~/Documents$ cat food.txt
```

Food is good.
Although the terminal is the default output of this command, the cat command can also be used for redirecting file content to other files or input for another command by using redirection characters.

#### 10.1.2 Viewing Files Using a Pager

While viewing small files with the cat command poses no problems, it is not an ideal choice for large files. The cat command doesn't provide any easy ways to pause and restart the display, so the entire file contents are dumped to the screen.
For larger files, use a pager command to view the contents. Pager commands display one page of data at a time, allowing you to move forward and backward in the file by using movement keys.
There are two commonly used pager commands:
- The less command provides a very advanced paging capability. It is usually the default pager used by commands like the man command.
- The more command has been around since the early days of UNIX. While it has fewer features than the less command, however, the less command isn't included with all Linux distributions. The more command is always available.
The more and less commands allow users to move around the document using keystroke commands. Because developers based the less command on the functionality of the more command, all of the keystroke commands available in the more command also work in the less command.
The focus of our content is on the more advanced less command. The more command is still useful to remember for times when the less command isn't available. Remember that most of the keystroke commands provided work for both commands.

##### 10.1.2.1 Pager Movement Commands

To view a file with the less command, pass the file name as an argument:

```text
sysadmin@localhost:~/Documents$ less words
```

There are many movement commands for the less command, each with multiple possible keys or key combinations. While this may seem intimidating, it is not necessary to memorize all of these movement commands. When viewing a file with the less command, use the H key or Shift+H to display a help screen:
SUMMARY OF LESS COMMANDS

Commands marked with * may be preceded by a number, N.
Notes in parentheses indicate the behavior if N is given.
A key preceded by a caret indicates the Ctrl key; thus ^K is ctrl-K.

h  H                 Display this help.
q  :q  Q  :Q  ZZ     Exit.
------------------------------------------------------------------------
MOVING

e  ^E  j  ^N  CR  *  Forward  one line   (or N lines).
y  ^Y  k  ^K  ^P  *  Backward one line   (or N lines).
f  ^F  ^V  SPACE  *  Forward  one window (or N lines).
b  ^B  ESC-v      *  Backward one window (or N lines).
z                 *  Forward  one window (and set window to N).
w                 *  Backward one window (and set window to N).
ESC-SPACE         *  Forward  one window, but don't stop at end-of-file.
d  ^D             *  Forward  one half-window (and set half-window to N).
u  ^U             *  Backward one half-window (and set half-window to N).
ESC-)  RightArrow *  Left  one half screen width (or N positions).
ESC-(  LeftArrow  *  Right one half screen width (or N positions).
HELP -- Press RETURN for more, or q when done
The first group of movement commands to focus on are the ones that are most commonly used. To make it even more convenient, the keys that are identical in more and less are summarized below in order to demonstrate how to move in more and less at the same time:
Key	Movement
Spacebar	Window forward
B	Window backward
Enter	Line forward
Q	Exit
H	Help
When using less as a pager, the easiest way to advance forward a page is to press the Spacebar.

### 10.2 Command Line Pipes

The pipe | character can be used to send the output of one command to another. Typically, when a command has output or generates an error, the output is displayed to the screen; however, this does not have to be the case. Instead of being printed to the screen, the output of one command becomes input for the next command. This tool can be powerful, especially when looking for specific data; piping is often used to refine the results of an initial command.
In previous examples the head and tail commands were given files as arguments to operate on. However, the pipe character allows you to utilize these commands not only on files, but on the output of other commands. This can be useful when listing a large directory, for example the /etc directory:

```text
sysadmin@localhost:~$ ls /etc
```

X11                     gss              mke2fs.conf     rpc
adduser.conf            host.conf        modprobe.d      rsyslog.conf
alternatives            hostname         modules         rsyslog.d
apparmor                hosts            modules-load.d  securetty
apparmor.d              hosts.allow      motd            security
apt                     hosts.deny       mtab            selinux
bash.bashrc             init.d           nanorc          services
bind                    initramfs-tools  netplan         shadow
bindresvport.blacklist  inputrc          network         shadow-
binfmt.d                insserv.conf.d   networks        shells
ca-certificates         iproute2         newt            skel
ca-certificates.conf    issue            nsswitch.conf   ssh
calendar                issue.net        opt             ssl
console-setup           kernel           os-release      subgid
cron.d                  ld.so.cache      pam.conf        subgid-
cron.daily              ld.so.conf       pam.d           subuid
cron.hourly             ld.so.conf.d     passwd          subuid-
cron.monthly            ldap             passwd-         sudoers
cron.weekly             legal            perl            sudoers.d
crontab                 libaudit.conf    pinforc         sysctl.conf
dbus-1                  locale.alias     ppp             sysctl.d
debconf.conf            locale.gen       profile         systemd
debian_version          localtime        profile.d       terminfo
default                 logcheck         protocols       timezone
deluser.conf            login.defs       python3         tmpfiles.d
depmod.d                logrotate.conf   python3.6       ucf.conf
dhcp                    logrotate.d      rc0.d           udev
dpkg                    lsb-release      rc1.d           ufw
environment             machine-id       rc2.d           update-motd.d
fstab                   magic            rc3.d           updatedb.conf
gai.conf                magic.mime       rc4.d           vim
groff                   mailcap          rc5.d           vtrgb
group                   mailcap.order    rc6.d           wgetrc
group-                  manpath.config   rcS.d           xdg
gshadow                 mc               resolv.conf
gshadow-                mime.types       rmt
The previous command lists a large number of files. If you execute this in our terminal, the output is cut off and can only be viewed if scrolling up. To more easily view the beginning of the output, pipe it to the head command. The following example displays only the first ten lines:

```text
sysadmin@localhost:~$ ls /etc | head
```

X11
adduser.conf
alternatives
apparmor
apparmor.d
apt
bash.bashrc
bind
bindresvport.blacklist
binfmt.d
The full output of the ls command is passed to the head command by the shell instead of being printed to the screen. The head command takes this output from the ls command as input data, and the output of head is then printed to the screen.
Multiple pipes can be used consecutively to link multiple commands together. If three commands are piped together, the output of the first command is passed to the second command. Then, the output of the second command is passed to the third command. The output of the third command would then be printed to the screen.
It is important to carefully choose the order in which commands are piped, as each command only sees input from the previous command. The examples below illustrate this using the nl command, which adds line numbers to the output. In the first example, the nl command is used to number the lines of the output of the preceding ls command:

```text
sysadmin@localhost:~$ ls /etc/ssh | nl

## 1 moduli

## 2 ssh_config

## 3 ssh_host_ecdsa_key

## 4 ssh_host_ecdsa_key.pub

## 5 ssh_host_ed25519_key

## 6 ssh_host_ed25519_key.pub

## 7 ssh_host_rsa_key

## 8 ssh_host_rsa_key.pub

## 9 ssh_import_id

## 10 sshd_config

```

In the next example, note that the ls command is executed first and its output is sent to the nl command, numbering all of the lines from the output of the ls command. Then the tail command is executed, displaying the last five lines from the output of the nl command:

```text
sysadmin@localhost:~$ ls /etc/ssh | nl | tail -5

## 6 ssh_host_ed25519_key.pub

## 7 ssh_host_rsa_key

## 8 ssh_host_rsa_key.pub

## 9 ssh_import_id

## 10 sshd_config

```

Compare the output above with the next example:

```text
sysadmin@localhost:~$ ls /etc/ssh | tail -5 | nl

## 1 ssh_host_ed25519_key.pub

## 2 ssh_host_rsa_key

## 3 ssh_host_rsa_key.pub

## 4 ssh_import_id

## 5 sshd_config

```

Notice how the line numbers are different. Why is this?
In the second example, the output of the ls command is first sent to the tail command which only grabs the last five lines of the output. Then the tail command sends those five lines to the nl command, which numbers them 1-5.
Pipes can be powerful, but it is necessary to consider how commands are piped to ensure that the desired output is displayed.

### 10.3 Input/Output Redirection

Input/Output (I/O) redirection allows for command line information to be passed to different streams. Before discussing redirection, it is important to understand the standard streams.
1. STDIN
Standard input, or STDIN, is information entered normally by the user via the keyboard. When a command prompts the shell for data, the shell provides the user with the ability to type commands that, in turn, are sent to the command as STDIN.
1. STDOUT
Standard output, or STDOUT, is the normal output of commands. When a command functions correctly (without errors) the output it produces is called STDOUT. By default, STDOUT is displayed in the terminal window where the command is executing. STDOUT is also known as stream or channel #1.
1. STDERR
Standard error, or STDERR, is error messages generated by commands. By default, STDERR is displayed in the terminal window where the command is executing. STDERR is also known as stream or channel #2.
I/O redirection allows the user to redirect STDIN so that data comes from a file and STDOUT/STDERR so that output goes to a file. Redirection is achieved by using the arrow < > characters.

### 10.4 Sorting Files or Input

The sort command can be used to rearrange the lines of files or input in either dictionary or numeric order. The following example creates a small file, using the head command to grab the first 5 lines of the /etc/passwd file and send the output to a file called mypasswd.

```text
sysadmin@localhost:~$ head -5 /etc/passwd > mypasswd
sysadmin@localhost:~$ cat mypasswd
```

root:x:0:0:root:/root:/bin/bash
daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
bin:x:2:2:bin:/bin:/usr/sbin/nologin
sys:x:3:3:sys:/dev:/usr/sbin/nologin
sync:x:4:65534:sync:/bin:/bin/sync
Now we will sort the mypasswd file:

```text
sysadmin@localhost:~$ sort mypasswd
```

bin:x:2:2:bin:/bin:/usr/sbin/nologin
daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
root:x:0:0:root:/root:/bin/bash
sync:x:4:65534:sync:/bin:/bin/sync
sys:x:3:3:sys:/dev:/usr/sbin/nologin
Upon close examination of the output in the preceding example, the sort command has arranged the lines of the file in alphabetical order. Compare this output to the output of the previous cat command.

#### 10.4.1 Fields and Sort Options

The sort command can rearrange the output based on the contents of one or more fields. Fields are determined by a field delimiter contained on each line. In computing, a delimiter is a character that separates a string of text or data; it defaults to whitespace, like spaces or tabs.
The following command can be used to sort the third field of the mypasswd file numerically. Three options are used to achieve this sort:
Option	Function
-t:	The -t option specifies the field delimiter. If the file or input is separated by a delimiter other than whitespace, for example a comma or colon, the -t option will allow for another field separator to be specified as an argument.
The mypasswd file used in the previous example uses a colon : character as a delimiter to separate the fields, so the following example uses the -t: option.

```text
-k3	The -k option specifies the field number. To specify which field to sort by, use the -k option with an argument to indicate the field number, starting with 1 for the first field.
```

The following example uses the -k3 option to sort by the third field.

```text
-n	This option specifies the sort type.
```

The third field in the mypasswd file contains numbers, so the -n option is used to perform a numeric sort.

```text
sysadmin@localhost:~$ sort -t: -n -k3 mypasswd
```

root:x:0:0:root:/root:/bin/bash
daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
bin:x:2:2:bin:/bin:/usr/sbin/nologin
sys:x:3:3:sys:/dev:/usr/sbin/nologin
sync:x:4:65534:sync:/bin:/bin/sync
Another commonly used option to the sort command is the -r option, which is used to perform a reverse sort. The following shows the same command as the previous example, with the addition of the -r option, making the higher numbers in the third field appear at the top of the output:

```text
sysadmin@localhost:~$ sort -t: -n -r -k3 mypasswd
```

sync:x:4:65534:sync:/bin:/bin/sync
sys:x:3:3:sys:/dev:/usr/sbin/nologin
bin:x:2:2:bin:/bin:/usr/sbin/nologin
daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
root:x:0:0:root:/root:/bin/bash
Lastly, you may want to perform more complex sorts, such as sorting by a primary field and then by a secondary field. For example, consider the following comma-separated value file, a file where the comma character is the field delimiter:
Follow Along
Use the following command to switch to the Documents directory:

```text
sysadmin@localhost:~$ cd ~/Documents
sysadmin@localhost:~/Documents$ cat os.csv
```

1970,Unix,Richie
1987,Minix,Tanenbaum
1970,Unix,Thompson
1991,Linux,Torvalds
To sort first by the operating system (field #2) and then year (field #1) and then by last name (field #3), use the following command:

```text
sysadmin@localhost:~/Documents$ sort -t, -k2 -k1n -k3 os.csv
```

1991,Linux,Torvalds
1987,Minix,Tanenbaum
1970,Unix,Richie
1970,Unix,Thompson
The following table breaks down the options used in the previous example:
Option	Function
-t,	Specifies the comma character as the field delimiter

```text
-k2	Sort by field #2
-k1n	Numerically sort by field #1
-k3	Sort by field #3
```

Use the following command to return to the home directory:

```text
sysadmin@localhost:~/Documents$ cd
sysadmin@localhost:~$

### 10.5 Viewing File Statistics

```

The wc command provides the number of lines, words and bytes (1 byte = 1 character in a text file) for a file, and a total line count if more than one file is specified. By default, the wc command allows for up to three statistics to be printed for each file provided, as well as the total of these statistics if more than one filename is provided:

```text
sysadmin@localhost:~$ wc /etc/passwd /etc/passwd-

## 35 56 1710 /etc/passwd

## 34 55 1665 /etc/passwd-

## 69 111 3375 total

```

The output of the previous example has four columns:
1. Number of lines
2. Number of words
3. Number of bytes
4. File name
It is also possible to view only specific statistics, by using the -l option to show just the number of lines, the -w option to show just the number of words, the -c option to show just the number of bytes, or any combination of these options.
The wc command can be useful for counting the number of lines output by some other command through a pipe. For example, if you wanted to know the total number of files in the /etc directory, pipe the output of ls to wc and count only the number of lines:

```text
sysadmin@localhost:~$ ls /etc/ | wc -l
```

142

### 10.6 Filter File Sections

The cut command can extract columns of text from a file or standard input. It’s primarily used for working with delimited database files. Again, delimited files are files that contain columns separated by a delimiter. These files are very common on Linux systems.
By default, the cut command expects its input to be separated by the tab character, but the -d option can specify alternative delimiters such as the colon or comma.
The -f option can specify which fields to display, either as a hyphenated range or a comma-separated list.
In the following example, the first, fifth, sixth and seventh fields from the mypasswd database file are displayed:

```text
sysadmin@localhost:~$ cut -d: -f1,5-7 mypasswd
```

root:root:/root:/bin/bash
daemon:daemon:/usr/sbin:/usr/sbin/nologin
bin:bin:/bin:/usr/sbin/nologin
sys:sys:/dev:/usr/sbin/nologin
sync:sync:/bin:/bin/sync
The cut command is also able to extract columns of text based upon character position with the -c option—useful when working with fixed-width database files or command outputs.
For example, the fields of the ls -l command are always in the same character positions. The following will display just the file type (character 1), permissions (characters 2-10), a space (character 11), and filename (characters 50+):

```text
sysadmin@localhost:~$ ls -l | cut -c1-11,50-
```

total 44
drwxr-xr-x Desktop
drwxr-xr-x Documents
drwxr-xr-x Downloads
drwxr-xr-x Music
drwxr-xr-x Pictures
drwxr-xr-x Public
drwxr-xr-x Templates
drwxr-xr-x Videos

```text
-rw-rw-r-- all.txt
-rw-rw-r-- example.txt
-rw-rw-r-- mypasswd
-rw-rw-r-- new.txt

### 10.7 Filter File Contents

```

The grep command can be used to filter lines in a file or the output of another command that matches a specified pattern. That pattern can be as simple as the exact text that you want to match or it can be much more advanced through the use of regular expressions.
For example, to find all the users who can log in to the system with the BASH shell, the grep command can be used to filter the lines from the /etc/passwd file for the lines containing the pattern bash:

```text
sysadmin@localhost:~$ grep bash /etc/passwd
```

root:x:0:0:root:/root:/bin/bash
sysadmin:x:1001:1001:System Administrator,,,,:/home/sysadmin:/bin/bash
To make it easier to see what exactly is matched, use the --color option. This option will highlight the matched items in red:

```text
sysadmin@localhost:~$ grep --color bash /etc/passwd
```

root:x:0:0:root:/root:/bin/bash
sysadmin:x:1001:1001:System Administrator,,,,:/home/sysadmin:/bin/bash

> **Note**
>
On our virtual machines, the grep command is aliased to include the --color option automatically.
In some cases, it may not be important to find the specific lines that match the pattern, but rather how many lines match the pattern. The -c option provides a count of how many lines match:

```text
sysadmin@localhost:~$ grep -c bash /etc/passwd
```

2
When viewing the output from the grep command, it can be hard to determine the original line numbers. This information can be useful when going back into the file (perhaps to edit the file) to quickly find one of the matched lines.
The -n option to the grep command will display original line numbers. To display all lines and their line numbers in the /etc/passwd file which contain the pattern bash:

```text
sysadmin@localhost:~$ grep -n bash /etc/passwd
```

1:root:x:0:0:root:/root:/bin/bash
27:sysadmin:x:1001:1001:System Administrator,,,,:/home/sysadmin:/bin/bash
The -v option inverts the match, outputting all lines that do not contain the pattern. To display all lines not containing nologin in the /etc/passwd file:

```text
sysadmin@localhost:~$ grep -v nologin /etc/passwd
```

root:x:0:0:root:/root:/bin/bash
sync:x:4:65534:sync:/bin:/bin/sync
operator:x:1000:37::/root:/bin/sh
sysadmin:x:1001:1001:System Administrator,,,,:/home/sysadmin:/bin/bash
The -i option ignores the case (capitalization) distinctions. The following searches for the pattern the in newhome.txt, allowing each character to be uppercase or lowercase:

```text
sysadmin@localhost:~$ cd Documents
sysadmin@localhost:~/Documents$ grep -i the newhome.txt
```

There are three bathrooms.
**Beware** of the ghost in the bedroom.
The kitchen is open for entertaining.
**Caution** the spirits don't like guests.
The -w option only returns lines which contain matches that form whole words. To be a word, the character string must be preceded and followed by a non-word character. Word characters include letters, digits, and the underscore character.
The following examples search for the are pattern in the newhome.txt file. The first command searches with no options, while the second command includes the -w option. Compare the outputs:

```text
sysadmin@localhost:~/Documents$ grep are newhome.txt
```

There are three bathrooms.
**Beware** of the ghost in the bedroom.

```text
sysadmin@localhost:~/Documents$ grep -w are newhome.txt
```

There are three bathrooms.

### 10.8 Basic Regular Expressions

Regular expressions, also referred to as regex, are a collection of normal and special characters that are used to find simple or complex patterns, respectively, in files. These characters are characters that are used to perform a particular matching function in a search.
Normal characters are alphanumeric characters which match themselves. For example, an a would match an a. Special characters have special meanings when used within patterns by commands like the grep command. They behave in a more complex manner and do not match themselves.
There are both Basic Regular Expressions (available to a wide variety of Linux commands) and Extended Regular Expressions (available to more advanced Linux commands). Basic Regular Expressions include the following:
Character	Matches
.	Any single character
[ ]	A list or range of characters to match one character
If the first character within the brackets is the caret ^, it means any character not in the list
*	The previous character repeated zero or more times
^	If the first character in the pattern, the pattern must be at the beginning of the line to match, otherwise just a literal ^ character
$	If the last character in the pattern, the pattern must be at the end of the line to match, otherwise just a literal $ character
The grep command is just one of the many commands that support regular expressions. Some other commands include the more and less commands.
While some of the regular expressions are unnecessarily quoted with single quotes, it is good practice to use single quotes around regular expressions to prevent the shell from trying to interpret special meaning from them.

#### 10.8.1 The Period . Character

One of the most useful expressions is the period . character. It matches any character except for the new line character. Consider the unfiltered contents of the ~/Documents/red.txt file:

```text
sysadmin@localhost:~/Documents$ cat red.txt
```

red
reef
rot
reeed
rd
rod
roof
reed
root
reel
read
The pattern r..f would find any line that contained the letter r followed by exactly two characters and then the letter f:

```text
sysadmin@localhost:~/Documents$ grep 'r..f' red.txt
```

reef
roof
The line does not have to be an exact match, it simply must contain the pattern, as seen here when r..t is searched for in the /etc/passwd file:

```text
sysadmin@localhost:~/Documents$ grep 'r..t' /etc/passwd
```

root:x:0:0:root:/root:/bin/bash
operator:x:1000:37::/root:
The period character can be used any number of times. To find all words that have at least four characters, the following pattern can be used:

```text
sysadmin@localhost:~/Documents$ grep '....' red.txt
```

reef
reeed
roof
reed
root
reel
read

#### 10.8.6 Extended Regular Expressions

The use of extended regular expressions often requires a special option be provided to the command to recognize them. Historically, there is a command called egrep, which is similar to grep, but can understand extended regular expressions. Now, the egrep command is deprecated in favor of using grep with the -E option.
The following regular expressions are considered extended:
Character	Meaning
?	Matches previous character zero or one time, so it is an optional character
+	Matches previous character repeated one or more times
|	Alternation or like a logical "or" operator
To match colo followed by zero or one u character followed by an r character:

```text
sysadmin@localhost:~/Documents$ grep -E 'colou?r' spelling.txt
```

American English: Do you consider gray to be a color or a shade?
British English: Do you consider grey to be a colour or a shade?
To match one or more e characters:

```text
sysadmin@localhost:~/Documents$ grep -E 'e+' red.txt
```

red
reef
reeed
reed
reel
read
To match either gray or grey:

```text
sysadmin@localhost:~/Documents$ grep -E 'gray|grey' spelling.txt
```

American English: Do you consider gray to be a color or a shade?
British English: Do you consider grey to be a colour or a shade?

### 11.1 Introduction

In this chapter, we will discuss how the tools you have learned so far can be turned into reusable scripts.

### 11.2 Shell Scripts in a Nutshell

A shell script is a file of executable commands that has been stored in a text file. When the file is run, each command is executed. Shell scripts have access to all the commands of the shell, including logic. A script can therefore test for the presence of a file or look for particular output and change its behavior accordingly. You can build scripts to automate repetitive parts of your work, which frees your time and ensures consistency each time you use the script. For instance, if you run the same five commands every day, you can turn them into a shell script that reduces your work to one command.
A script can be as simple as one command:
echo "Hello, World!"
The script, test.sh, consists of just one line that prints the string Hello, World! to the console.

> **Note**
>
This file is not available within the virtual machine environment of this course.
Running a script can be done either by passing it as an argument to your shell or by running it directly:

```text
sysadmin@localhost:~$ sh test.sh
```

Hello, World!

```text
sysadmin@localhost:~$ ./test.sh
```

-bash: ./test.sh: Permission denied

```text
sysadmin@localhost:~$ chmod +x ./test.sh
sysadmin@localhost:~$ ./test.sh
```

Hello, World!
In the example above, first, the script is run as an argument to the shell. Next, the script is run directly from the shell. It is rare to have the current directory in the binary search path $PATH so the name is prefixed with ./ to indicate that it should be run out of the current directory.
The error Permission denied means that the script has not been marked as executable. A quick chmod later and the script works. chmod is used to change the permissions of a file, which will be explained in detail in a later chapter.
There are various shells with their own language syntax. Therefore, more complicated scripts will indicate a particular shell by specifying the absolute path to the interpreter as the first line, prefixed by #! as shown:
#!/bin/sh
echo "Hello, World!"
or
#!/bin/bash
echo "Hello, World!"
The two characters #! are traditionally called the hash and the bang respectively, which leads to the shortened form of “shebang” when they’re used at the beginning of a script.
Incidentally, the shebang (or crunchbang) is used for traditional shell scripts and other text-based languages like Perl, Ruby, and Python. Any text file marked as executable will be run under the interpreter specified in the first line as long as the script is run directly. If the script is invoked directly as an argument to an interpreter, such as sh script or bash script, the given shell will be used no matter what’s in the shebang line.
It helps to become comfortable using a text editor before writing shell scripts, since you will need to create files in plain text. Traditional office tools like LibreOffice that output file formats containing formatting and other information are not appropriate for this task.

### 11.3 Editing Shell Scripts

UNIX has many text editors. The merits of one over the other are often hotly debated. Two are specifically mentioned in the LPI Essentials syllabus: The GNU nano editor is a very simple editor well suited to editing small text files. The Visual Editor, vi, or its newer version, VI improved (vim), is a remarkably powerful editor but has a steep learning curve. We’ll focus on nano.
Type nano test.sh and you’ll see a screen similar to this:
GNU nano 2.2.6              File: test.sh                         modified

#!/bin/sh

echo "Hello, World!"
echo -n "the time is "
date

^G Get Help  ^O WriteOut  ^R Read File ^Y Prev Page ^K Cut Text  ^C Cur Po
^X Exit      ^J Justify   ^W Where Is  ^V Next Page ^U UnCut Text^T To Spell
The nano editor has few features to get you on your way. You simply type with your keyboard, using the arrow keys to move around and the delete/backspace button to delete text. Along the bottom of the screen you can see some commands available to you, which are context-sensitive and change depending on what you’re doing. If you’re directly on the Linux machine itself, as opposed to connecting over the network, you can also use the mouse to move the cursor and highlight text.
To get familiar with the editor, start typing out a simple shell script while inside nano:
GNU nano 2.2.6              File: test.sh                         modified

#!/bin/sh

echo "Hello, World!"
echo -n "the time is "
date

^G Get Help  ^O WriteOut  ^R Read File ^Y Prev Page ^K Cut Text  ^C Cur Po
^X Exit      ^J Justify   ^W Where Is  ^V Next Page ^U UnCut Text^T To Spell
Note that the bottom-left option is ^X Exit which means “press control and X to exit”. Press Ctrl and X together and the bottom will change:
Save modified buffer (ANSWERING "No" WILL DESTROY CHANGES) ?
Y Yes
N No           ^C Cancel
At this point, you can exit the program without saving by pressing the N key, or save first by pressing Y to save. The default is to save the file with the current file name. You can press the Enter key to save and exit.
You will be back at the shell prompt after saving. Return to the editor. This time press Ctrl and O together to save your work without exiting the editor. The prompts are largely the same, except that you’re back in the editor.
This time use the arrow keys to move your cursor to the line that has "The time is”. Press Control and K twice to cut the last two lines to the copy buffer. Move your cursor to the remaining line and press Control and U once to paste the copy buffer to the current position. This makes the script echo the current time before greeting you and saved you needing to re-type the lines.
Other helpful commands you might need are:
Command	Description
Ctrl + W 	search the document
Ctrl + W, then Control + R 	search and replace
Ctrl + G 	show all the commands possible
Ctrl + Y/V 	page up / down
Ctrl + C 	show the current position in the file and the file’s size

### 11.4 Scripting Basics

You got your first taste of scripting earlier in this chapter where we introduced a very basic script that ran a single command. The script started with the shebang (or hashbang) line, telling Linux that /bin/bash (which is Bash) is to be used to execute the script.
Other than running commands, there are 3 topics you must become familiar with:
1. Variables, which hold temporary information in the script
2. Conditionals, which let you do different things based on tests you write
3. Loops, which let you do the same thing over and over

### 12.1 Introduction

Computers begin as a hardware device but can grow to encompass virtual machines that are entirely constructed out of software and appear to all purposes to be a remote machine that users can access via remote protocols and methods.
Keeping virtual machines in mind, it’s imperative to understand what makes up the physical hardware that makes up a computer. Without an understanding of what components make up a computer, how they are integrated and communicate between each other, and how a computer should function, you cannot properly install, configure, administer, secure or troubleshoot a system.
There are hundreds of specific types of computers in service, from set-top boxes to dedicated firewalls to laptops, servers and many special-purpose devices, but they all feature at least a few of the same basic components that actually make them a computer. This chapter introduces and explains the basics of what makes up a computer and expands to a few optional items that are fairly commonplace.

### 12.2 Motherboards

The motherboard, or system board, is the main hardware board in the computer through which the central processing unit (CPU), random-access memory (RAM) and other components are all connected. Depending on the computer type (laptop, desktop, server) some devices, such as processors and RAM, are attached directly to the motherboard, while other devices, such as add-on cards, are connected via a bus.

### 12.3 Processors

A central processing unit (CPU or processor) is one of the most critical hardware components of a computer. The processor is the brain of the computer, where the execution of code takes place and where most calculations are done. It is directly connected (soldered) to the motherboard, as motherboards are typically configured to work with specific types of processors.
If a hardware system has more than one processor, the system is referred to as a multiprocessor. If more than one processor is combined into a single overall processor chip, then it is called multi-core.
Although support is available for more types of processors in Linux than any other operating system, there are primarily just two types of processors used on desktop and server computers: x86 and x86_64. On an x86 system, the system processes data 32 bits at a time; on an x86_64 the system processes data 64 bits at a time. An x86_64 system is also capable of processing data 32 bits at a time in a backward compatible mode. One of the main advantages of a 64-bit system is the ability to work with more memory, while other advantages include increased efficiency of processing and increased security.
Intel originated the x86 family of processors in 1978 with the release of the 8086 processor. Since that time, Intel has produced many other processors that are improvements to the original 8086; they are known generically as x86 processors. These processors include the 80386 (i386), 80486 (i486), the Pentium series (i586) and the Pentium Pro series (i686). In addition to Intel, other companies such as AMD and Cyrix have also produced x86 compatible processors. While Linux is capable of supporting processors back to the i386 generation, many distributions (especially the ones that feature corporate support, such as SUSE, Red Hat and Canonical) limit their support to i686 or later.
The x86_64 family of processors, including the 64-bit processors from Intel and AMD, have been in production since around the year 2000. As a result, almost all of the modern processors shipped today are of the x86_64 type. While the hardware has been available for over a decade now, the software to support this family of processors has been much slower to develop. Although it’s 2018 at the time of this update, there remain a number of packages that are still available for the x86 architecture.
To see which family the CPU of the current system belongs to, use the arch command:

```text
sysadmin@localhost:~$ arch
```

x86_64
For more information concerning the CPU, use the lscpu command:

```text
sysadmin@localhost:~$ lscpu
```

Architecture:          x86_64
CPU op-mode(s):        32-bit, 64-bit
Byte Order:            Little Endian
CPU(s):                4
On-line CPU(s) list:   0-3
Thread(s) per core:    1
Core(s) per socket:    4
Socket(s):             1
NUMA node(s):          1
Vendor ID:             GenuineIntel
The first line of this output shows that the CPU is being used in a 64-bit mode, as the architecture reported is x86_64. The second line of output shows that the CPU is capable of operating in either a 32- or 64-bit mode, therefore, it is actually a 64-bit CPU.

### 12.4 Random Access Memory

The motherboard typically has slots where random-access memory (RAM) can be connected to the system. The 32-bit architecture systems can use up to 4 gigabytes (GB) of RAM, while 64-bit architectures are capable of addressing and using far more RAM.
In some cases, the RAM a system has might not be enough to handle all of the operating system requirements. Once invoked, programs are loaded in RAM along with any data they need to store, while instructions are sent to the processor when they execute.
When the system is running low on RAM, virtualized memory called swap space is used to temporarily store data to disk. Data stored in RAM that has not been used recently is moved over to the section of the hard drive designated as swap, freeing up more RAM for use by currently active programs. If needed, this swapped data can be moved back into RAM at a later time. The system does all of this automatically as long as swap is configured.
To view the amount of RAM in your system, including the swap space, execute the free command. The free command has a -m option to force the output to be rounded to the nearest megabyte (MB) and a -g option to force the output to be rounded to the nearest gigabyte (GB):

```text
sysadmin@localhost:~$ free -m
```

total       used       free     shared    buffers     cached
Mem:          1894        356       1537          0          25       177
-/+ buffers/cache:        153       1741
Swap:         4063          0       4063
The output shows that this system has a total of 1,894 MB and is currently using 356 MB.
The amount of swap appears to be approximately 4 GB, although none of it appears to be in use. This makes sense because so much of the physical RAM is free, so there is no need at this time for virtual RAM (swap space) to be used.

### 12.5 Buses

A bus is a high-speed connection that allows communication between computers or the components inside a computer. The motherboard has buses that allow for multiple devices to connect to the system, including the Peripheral Component Interconnect (PCI) and Universal Serial Bus (USB). The motherboard also has connectors for monitors, keyboards and mice.
Different system types will use a bus differently to connect components. In a desktop or server computer, there is a motherboard with the processor, RAM, and other components directly attached, and then a high-speed bus that allows additional components to be attached via card slots, such as video, network and other peripheral devices.
Increasingly for laptop and light/thin/small form factor computers, the majority of the computer’s components may be directly connected to the motherboard, including the usual processor, RAM, as well as additional components like the network card. In this configuration, the bus still exists, but effectively one of the main convenience factors of being able to swap out or upgrade devices is no longer a possibility.
Peripheral Devices
Peripheral devices are components connected to a computer that allow input, output or data storage. Keyboards, mice, monitors, printers and hard disks are all considered peripherals and are accessed by the system in order to perform functions outside of central processing. To view all of the devices connected by the PCI bus, the user can execute the lspci command. The following is a sample output of this command. The highlighted sections show this system has a VGA controller (a monitor connector), an SCSI storage controller (a type of hard drive) and an Ethernet controller (a network connector):

> **Note**
>
The example below uses the lspci command. This command is not available within the virtual machine environment of this course.

```text
sysadmin@localhost:~$ lspci
```

00:00.0 Host bridge: Intel Corporation 440BX/ZX/DX - 82443BX/ZX/DX Host bridge (rev 01)
00:01.0 PCI bridge: Intel Corporation 440BX/ZX/DX - 82443BX/ZX/DX AGP bridge (rev 01)
00:07.0 ISA bridge: Intel Corporation 82371AB/EB/MB PIIX4 ISA (rev 08)
00:07.1 IDE interface: Intel Corporation 82371AB/EB/MB PIIX4 IDE (rev 01)
00:07.3 Bridge: Intel Corporation 82371AB/EB/MB PIIX4 ACPI (rev 08)
00:07.7 System peripheral: VMware Virtual Machine Communication Interface (rev 10)
00:0f.0 VGA compatible controller: VMware SVGA II Adapter
03:00.0 Serial Attached SCSI controller: VMware PVSCSI SCSI Controller (rev 02
0b:00.0 Ethernet controller: VMware VMXNET3 Ethernet Controller (rev 01)
Universal Serial Bus Devices
While the PCI bus is used for many internal devices such as sound and network cards, an ever-increasing number of external devices (or peripherals) are connected to the computer via USB.
Devices connected internally are usually cold-plug, meaning the system must be shut down in order to connect or disconnect a device. USB devices are hot-plug, meaning they can be connected or disconnected while the system is running.
Though USB devices are hot-plug by design, it's important to ensure that any mounted filesystems are correctly unmounted, or data loss and corruption of the filesystem may occur.
To display the devices connected to the system via USB, execute the lsusb command:

> **Note**
>
The example uses the lsusb command. This command is not available within the virtual machine environment of this course.

```text
sysadmin@localhost:~$ lsusb
```

Bus 001 Device 002: ID 0e0f:000b VMware, Inc.
Bus 001 Device 001: ID 1d6b:0002 Linux Foundation 2.0 root hub
Bus 002 Device 004: ID 0e0f:0008 VMware, Inc.
Bus 002 Device 003: ID 0e0f:0002 VMware, Inc. Virtual USB Hub
Bus 002 Device 002: ID 0e0f:0003 VMware, Inc. Virtual Mouse
Bus 002 Device 001: ID 1d6b:0001 Linux Foundation 1.1 root hub

### 12.6 Hard Drives

Hard drives, also called hard disks, disk devices, or storage devices, may be attached to the system in a number of ways; the controller may be integrated into the motherboard, on a PCI card, or as a USB device. For the purposes of most Linux systems, a hard drive can generally be defined as any electromechanical or electronic storage device that holds data to be accessed by the system.
Hard drives are divided into one or more partitions. A partition is a logical division of a hard drive, designed to take a large amount of available storage space and break it up into smaller areas. While it is common on Microsoft Windows to have a single partition for each hard drive, on Linux distributions, multiple partitions per hard drive is common.
Some hard drives make use of a partitioning technology called Master Boot Record (MBR) while others make use of a partitioning type called GUID Partitioning Table (GPT). The MBR type of partitioning has been used since the early days of the Personal Computer (PC), and the GPT type has been available since the year 2000.
An old term used to describe an internal hard disk is fixed disk, as the disk is fixed (not removable). This term gave rise to several command names: the fdisk, cfdisk and sfdisk commands, which are tools for working with the MBR partitioned disks.
The GPT disks use a newer type of partitioning, which allows the user to divide the disk into more partitions than what MBR supports. GPT also allows having partitions which can be larger than two terabytes (MBR does not). The tools for managing GPT disks are named similarly to their fdisk counterparts: gdisk, cgdisk, and sgdisk.
There is also a family of tools that attempt to support both MBR and GPT type disks. This set of tools includes the parted command and the graphical gparted tool.

> **Note**
>
Many Linux distributions use the gparted tool in the installation routine, as it provides a graphical interface to the powerful options available for creating new partitions, resizing existing ones (such as Windows partitions) and many other advanced tasks.
Hard drives are associated with file names (called device files) that are stored in the /dev directory. Each device file name is made up of multiple parts.
- File Type
The file name is prefixed based on the different types of hard drives. IDE (Intelligent Drive Electronics) hard drives begin with hd, while USB, SATA (Serial Advanced Technology Attachment) and SCSI (Small Computer System Interface) hard drives begin with sd.
- Device Order
Each hard drive is then assigned a letter which follows the prefix. For example, the first IDE hard drive would be named /dev/hda and the second would be /dev/hdb, and so on.
- Partition
Finally, each partition on a disk is given a unique numeric indicator. For example, if a USB hard drive has two partitions, they could be associated with the /dev/sda1 and /dev/sda2 device files.
The following example shows a system that has three sd devices: /dev/sda, /dev/sdb and /dev/sdc. Also, there are two partitions on the first device, as evidenced by the /dev/sda1 and /dev/sda2 files, and one partition on the second device, as evidenced by the /dev/sdb1 file:

```text
root@localhost:~$ ls /dev/sd*
/dev/sda /dev/sda1  /dev/sda2  /dev/sdb  /dev/sdb1  /dev/sdc
```

The fdisk command can be used to display further information about the partitions:

> **Note**
>
The following command requires root access.

```text
root@localhost:~$ fdisk -l /dev/sda
```

Disk /dev/sda: 21.5 GB, 21474836480 bytes

## 255 heads, 63 sectors/track, 2610 cylinders, total 41943040 sectors

Units = sectors of 1 * 512 = 512 bytes
Sector size (logical/physical): 512 bytes / 512 bytes
I/O size (minimum/optimal): 512 bytes / 512 bytes
Disk identifier: 0x000571a2

⁠⁠​ ⁠
Device Boot      Start         End      Blocks   Id  System

```text
/dev/sda1   *        2048    39845887    19921920   83  Linux
/dev/sda2        39847934    41940991     1046529    5  Extended
/dev/sda5        39847936    41940991     1046528   82  Linux swap / Solaris

> **Note**
>
```

Creating and modifying partitions is beyond the scope of this course. For more information, check out NDG Linux I.

### 12.7 Solid State Disks

While the phrase hard disk is typically considered to encompass traditional spinning disk devices, it can also refer to the newer and very different solid state drives or disks.
Consider the difference between a traditional spinning platter hard disk and a USB thumb drive. The former literally has spinning disk platters in it that are read by drive heads, and the spinning disks are laid out to take advantage of the spinning nature of the device. Data is written (and read) in long strings of sequential blocks that a drive head encounters as the platter spins around.
Solid state disks are essentially larger capacity USB thumb drives in construction and function. As there are no moving parts, and no spinning disks, just memory locations to be read by the controller, a solid state disk is measurably and visibly faster in accessing the information stored in its memory chips.
A solid state disk is controlled by an embedded or onboard processor that makes the decisions as to where and how data is written and read back from the memory chips when requested.
Advantages of a solid state disk include lower power usage, time savings in system booting, faster program loads, and less heat and vibration from no moving parts. Disadvantages include higher costs in comparison to spinning hard disks, lower capacity due to the higher cost, and if soldered directly on the motherboard/mainboard, no ability to upgrade by swapping out the drive.

> **Note**
>
For the purposes of this course, and for understanding, we will refer to all disks, spinning or solid state, as hard disks unless there is an important distinction that requires us to differentiate between the two.

### 12.8 Optical Drives

Optical drives, often referred to as CD-ROMs, DVDs, or Blu-Ray, are removable storage media. While some devices used with optical disks are read-only, others are capable of burning (writing to) disks, when using a writable type of disk. There are various standards for writable and rewritable disks, such as CD-R, CD+R, DVD+RW, and DVD-RW.
Where these removable disks are mounted in the file system is an important consideration for a Linux administrator. Modern distributions often mount the disks under the /media folder, while older distributions typically mount them under the /mnt folder. For example, a USB thumb drive might be mounted on the /media/usbthumb path.
Upon mounting, most GUI interfaces prompt the user to take some action, such as open the contents of the disk in a file browser or start a media program. When the user is finished using the disk, it is necessary to unmount it using a menu or the umount command.

### 12.9 Managing Devices

```text
Linux by nature has a number of distributions or versions, a large portion of which are focused on mainstream hardware, while others run on relatively obscure types or models of hardware. It's safe to say that there is a Linux distribution specifically designed for just about all modern hardware platforms, and for many historical platforms as well.
```

Each of these hardware platforms has a great deal of variety in the components that are available. In addition to several different types of hard drives, there are many different graphics cards, monitors and printers. With the popularity of USB devices, such as USB storage devices, cameras, and mobile phones, the number of available devices you would want to connect to a Linux system can number in the thousands.
The sheer number of different devices poses problems as these hardware devices typically need drivers, software that allows them to communicate with the installed operating system.
The driver could be compiled as part of the Linux kernel, loaded into the kernel as a module, or loaded by a user command or application. External devices, like scanners and printers, typically have their drivers loaded by an application and these drivers, in turn, communicate through the device via the kernel through an interface such as USB.
Hardware manufacturers often provide this software, but typically for Microsoft Windows, not for Linux. This has been changing with the increasing popularity of Linux overall, but the desktop market share of Linux remains a very distant third to Microsoft and Apple systems.
Partly because there is relatively sparse vendor support, there is a great deal of community support from developers who strive to provide drivers for Linux systems. Although not all hardware has the necessary drivers, there is a decent amount that does, making the challenge for Linux users and administrators to either find the correct drivers or choose hardware that has some level of support in Linux.
In order to be successful in enabling devices in Linux, it is best to check the Linux distribution to see if the device is certified to work with that distribution. Commercial distributions like Red Hat and SUSE have web pages dedicated to listing hardware that is certified or approved to work with their software.
Additional tips on being successful with connecting your devices: avoid brand new or highly-specialized devices and check with the vendor of the device to see if they support Linux before making a purchase.

### 12.10 Video Display Devices

In order to display output to the monitor, the computer system must have a video display device (video card) and a monitor. Video display devices are often directly built into or attached to the motherboard, although they can also be connected through the PCI bus slots on the motherboard.
With the large array of video device vendors, each video display device usually requires a proprietary driver provided by the vendor. All drivers, but most especially video device drivers, must be written for the specific operating system, something that is commonly done for Microsoft Windows, but not always for Linux. Fortunately, most of the larger video display vendors now provide at least some level of Linux support. The Linux community has done an incredible amount of work developing standard drivers for video cards.

> **Note**
>
The video support issues that Linux has experienced are mostly focused on the desktop market for Linux. Server market share is mostly unaffected by the GUI, as the vast majority of Linux server implementations are text mode.
There are three types of video cables commonly used:
1. the older but still used analog 15-pin Video Graphics Array (VGA) cable
2. the more recent 29-pin Digital Visual Interface (DVI) interface
3. the very widely-used High-Definition Multimedia Interface (HDMI) which supports resolutions up to the 4K or Ultra HD range, and has either 19 or 29 pins
4. the newest digital display interface, the 20-pin DisplayPort (DP). Also its miniaturized counterpart, the Mini DisplayPort, used mainly for Apple products.
For monitors to work correctly with video display devices, they must be able to support the same resolution as the video display device. Normally, the software driving the video display device can automatically detect the maximum resolution that the video display and monitor can both support and set the screen resolution to that value.

### 12.11 Power Supplies

Power supplies are the devices that convert alternating current (120v, 240v) into direct current, which the computer uses at various voltages (3.3v, 5v, 12v). Power supplies are generally not programmable; however, their proper function has a major impact on the rest of the system.
Although they are not typically designed as surge suppressors, these devices often protect the computer from fluctuations in voltage coming from the power source. It is wise for a network administrator to choose a power supply based on quality rather than price since a failing power supply can result in significant damage to a computer system.
Desktop, server tower, rack and standalone systems are more vulnerable to power fluctuations than laptop systems are. If the power fluctuates, it can cause much havoc on the non-battery based systems, whereas a laptop simply keeps pulling power from its internal battery until depleted.

### 14.1 Introduction

Having access to the network is a key feature of most Linux systems. Users want to surf the net, send and receive email and transfer files with other users.
Typically the programs that perform these functions, such as web browsers and email clients, are reasonably easy to use. However, they all rely on an important feature: the ability of your computer to communicate with another computer. To have this communication, you need to know how to configure your system's network.

```text
Linux provides you with several tools to both configure your network as well as monitor how it is performing.‌⁠​​⁠​

### 14.2 Basic Network Terminology

```

Before setting up a network or accessing an existing network, it is beneficial to know some key terms that are related to networking. This section explores the terms with which you should be familiar. Some of the terms are basic, and you may already be familiar with them. However, others are more advanced.
Host	A host is a computer. Many people automatically think of a desktop computer or laptop when they hear the term computer. In reality, many other devices, such as cell phones, digital music players and many modern televisions, are also computers. In networking terms, a host is any device that communicates via a network with another device.
Network	A network is a collection of two or more hosts (computers) that are able to communicate with each other. This communication can be via a wired connection or wireless.
Internet	The Internet is an example of a network. It consists of a publicly accessible network that connects millions of hosts throughout the world. Many people use the Internet to surf web pages and exchange emails, but the Internet has many additional capabilities besides these activities.
Wi-Fi	The term Wi-Fi refers to wireless networks.
Server	A host that provides a service to another host or client is called a server. For example, a web server stores, processes and delivers web pages. An email server receives incoming mail and delivers outgoing mail.
Service	A feature provided by a host is a service. An example of a service would be when a host provides web pages to another host.
Client	A client is a host that is accessing a server. When you are working on a computer surfing the Internet, you are considered to be on a client host.
Router	Also called a gateway, a router is a machine that connects hosts from one network to another network. For example, if you work in an office environment, the computers within the company can all communicate via the local network created by the administrators. To access the Internet, the computers would have to communicate with a router that would be used to forward network communications to the Internet. Typically when you communicate on a large network (like the Internet), several routers are used before your communication reaches its final destination.

### 14.3 Networking Features Terminology

In addition to the networking terms discussed in the last section, there are some additional terms with which you should be familiar. These terms focus more on the different types of networking services that are commonly used, as well as some of the techniques that are used to communicate between machines.
Packet	A network packet is used to send network communication between hosts. By breaking down communication into smaller chunks (packets), the data delivery method is much more efficient.
IP Address	An Internet Protocol (IP) address is a unique number assigned to a host on a network. Hosts use these numbers to address network communication.
Mask	Also called a netmask, subnet mask or mask, a network mask is a number system that can be used to define which IP addresses are considered to be within a single network. Because of how routers perform their functions, networks have to be clearly defined.
Hostname	Each host on a network could have its own hostname because names are more natural for humans to remember than numbers, making it easier for us to address network packets to another host. Hostnames are translated into IP addresses before the network packet is sent on the network.
URL	A Uniform Resource Locator (URL), also commonly called a web address, is used to locate a resource, like a web page, on the internet. It’s what you type into your web browser to access a web page. For example, http://www.netdevgroup.com. It includes the protocol http:// and the hostname www.netdevgroup.com.
DHCP	Hosts can be assigned hostnames, IP addresses and other network-related information by a DHCP (Dynamic Host Configuration Protocol) server. In the world of computers, a protocol is a well-defined set of rules. DHCP defines how network information is assigned to client hosts, and the DHCP server is the machine that provides this information.
DNS	As mentioned previously, hostnames are translated into IP addresses, prior to the network packet being sent on the network. So your host needs to know the IP address of all of the other hosts with which you are communicating. When working on a large network (like the Internet), this can pose a challenge as there are so many hosts. A Domain Name System (DNS) provides the service of translating domain names into IP addresses.
Ethernet	In a wired network environment, Ethernet is the most common way to physically connect the hosts into a network. Ethernet cables are connected to network cards that support Ethernet connections. Ethernet cables and devices (such as routers) are specifically designed to support different communication speeds, the lowest being 10 Mbps (10 Megabits per second) and the highest being 100 Gbps (100 gigabits per second). The most common speeds are 100 Mbps and 1 Gbps.
TCP/IP	The Transmission Control Protocol/Internet Protocol (TCP/IP) is a fancy name for a collection of protocols (remember, protocol = set of rules) that are used to define how network communication should take place between hosts. While it isn't the only collection of protocols used to define network communication, it is the most often utilized one. As an example, TCP/IP includes the definition of how IP addresses and network masks work.

### 14.4 IP Addresses

As previously mentioned, hosts address network packets by using the IP address of the destination machine. The network packet also includes a return address, which is the IP address of the sending machine.
There are, in fact, two different types of IP addresses: IPv4 and IPv6. To understand why there are two different types, you need to understand a brief bit of IP addressing history.
For many years, the IP addressing technique that was used by all computers was IPv4. In an IPv4 address, a total of four 8-bit numbers are used to define the address. This is considered a 32-bit address (4 x 8 = 32). For example:
192.168.10.120
8-bit refers to numbers from 0 to 255.
Each host on the Internet must have a unique IP address. In an IPv4 environment, there is a technical limit of about 4.3 billion IP addresses. However, many of these IP addresses are not usable for various reasons. Also, many organizations haven't made use of all of the IP addresses they have available.
While it seems like there should be plenty of IP addresses to go around, various factors have led to a problem: the Internet started running out of IP addresses.
This issue encouraged the development of IPv6. IPv6 was officially created in 1998. In an IPv6 network the addresses are much larger, 128-bit addresses that look like this:
2001:0db8:85a3:0042:1000:8a2e:0370:7334
Essentially, this provides for a much larger address pool, so large that running out of addresses any time in the near future is very unlikely.
It is important to note that the difference between IPv4 and IPv6 isn't just a larger address pool. IPv6 has many other advanced features that address some of the limitations of IPv4, including better speed, more advanced package management and more efficient data transportation.
Considering all the advantages, you would think that by now all hosts would be using IPv6. However, the majority of network-attached devices in the world still use IPv4 (something like 98-99% of all devices).
So, why hasn't the world embraced the superior technology of IPv6?
There are primarily two reasons:
- NAT: Invented to overcome the possibility of running out of IP addresses in an IPv4 environment, Net Address Translation (NAT) used a technique to provide more hosts access to the Internet. In a nutshell, a group of hosts is placed into a private network with no direct access to the Internet; a special router provides Internet access, and only this one router needs an IP address to communicate on the Internet. In other words, a group of hosts shares a single IP address, meaning a lot more computers can attach to the Internet. This feature means the need to move to IPv6 is less critical than before the invention of NAT.
- Porting: Porting is switching over from one technology to another. IPv6 has a lot of great new features, but all of the hosts need to be able to utilize these features. Getting everyone on the Internet (or even just some) to make these changes poses a challenge.
Nonetheless, most experts agree that IPv6 will eventually replace IPv4, so understanding the basics of both is recommended for those who work in the IT industry.

### 14.5 Configuring Network Devices

When you are configuring network devices, there are two initial questions that you need to ask:
- Wired or wireless? Configuring a wireless device is slightly different to configuring a wired device because of some of the additional features typically found on wireless devices (such as security).
- DHCP or static address? Recall that a DHCP server provides network information, such as your IP address and subnet mask. If you don't make use of a DHCP server, then you will need to manually provide this information to your host, which is called using a static IP address.
Generally speaking, desktop machines use wired networks, while laptops use wireless networks. Normally a wired machine uses a static IP address, but these can also often be assigned via a DHCP server. In almost all cases, wireless machines use DHCP since they are almost always mobile and attached to different networks.

##### 14.5.1.1 Primary IPv4 Configuration File

On a CentOS system, the primary configuration file for an IPv4 network interface is the /etc/sysconfig/network-scripts/ifcfg-eth0 file. The VM in this chapter is Debian-based, and so does not have the sysconfig folder. However, for demonstration purposes only, the following shows what this file looks like when configured for a static IP address

```text
root@localhost:~# cat /etc/sysconfig/network-scripts/ifcfg-eth0
```

DEVICE="eth0"
BOOTPROTO=none
NM_CONTROLLED="yes"
ONBOOT=yes
TYPE="Ethernet"
UUID="98cf38bf-d91c-49b3-bb1b-f48ae7f2d3b5"
DEFROUTE=yes
IPV4 _FAILURE_FATAL=yes
IPV6INOT=no
NAME="System eth0"
IPADDR=192.168.1.1
PREFIX=24
GATEWAY=192.168.1.1
DNS1=192.168.1.2
HWADDR=00:50:56:90:18:18
LAST_CONNECT=1376319928
If the device were configured to be a DHCP client, the BOOTPROTO value would be set to dhcp, and the IPADDR, GATEWAY and DNS1 values would not be set.

##### 14.5.1.2 Primary IPv6 Configuration File

On a CentOS system, the primary IPv6 configuration file is the same file where IPv4 configuration is stored; the /etc/sysconfig/network-scripts/ifcfg-eth0 file. If you want to have your system have a static IPv6 address, add the following to the configuration file:
IPV6INIT=yes
IPV6ADDR=<IPv6 IP Address>
IPV6_DEFAULTGW=<IPv6 IP Gateway Address>
If you want your system to be a DHCP IPv6 client, then add the following setting:
DHCPV6C=yes
You also need to add the following setting to the /etc/sysconfig/network file:
NETWORKING_IPV6=yes

> **Consider This**
>
The widely accepted method of making changes to a network interface is to take the interface down using a command such as ifdown eth0, make the desired changes to the configuration file, and then bring the interface back up and into service with a command such as ifup eth0.
Another less specific method is to restart the system’s networking entirely, with a command such as service network restart, which takes down ALL interfaces, re-reads all related configuration files, and then restarts the networking for the system.
Restarting the network service can disrupt much more than just the single interface a user wanted to change, so use the most limited and specific commands to restart the interface if possible.
The following example demonstrates how the service command would need to be executed on a CentOS system:
[root@localhost ~]# service network restart
Shutting down interface eth0:  Device state: 3 (disconnected)
[  OK  ]
Shutting down loopback interface:                          [  OK  ]
Bringing up loopback interface:                            [  OK  ]
Bringing up interface eth0:  Active connection state: activated
Active connection path: /org/freedesktop/NetworkManager/ActiveConnection/1
[  OK  ]

##### 14.5.1.3 Domain Name System (DNS)

When a computer is asked to access a website, such as www.example.com, it does not necessarily know what IP address to use. For the computer to associate an IP address with the URL or hostname request, the computer relies upon the DNS service of another computer. Often, the IP address of the DNS server is discovered during the DHCP request, while a computer is receiving important addressing information to communicate on the network.
The address of the DNS server is stored in the /etc/resolv.conf file. A typical /etc/resolv.conf file is automatically generated and looks like the following:

```text
sysadmin@localhost:~$ cat /etc/resolv.conf
```

nameserver 127.0.0.1
The nameserver setting is often set to the IP address of the DNS server. The following example uses the host command, which works with DNS to associate a hostname with an IP address. Note that the example server is associated with the IP address 192.168.1.2 by the DNS server:

```text
sysadmin@localhost:~$ host example.com
```

example.com has address 192.168.1.2
It is also common to have multiple nameserver settings, in the event that one DNS server isn't responding.

##### 14.5.1.4 Network Configuration Files

Name resolution on a Linux host is accomplished by 3 critical files: the /etc/hosts, /etc/resolv.conf and /etc/nsswitch.conf files. Together, they describe the location of name service information, the order in which to check resources, and where to go for that information.
Files	Explanation

```text
/etc/hosts	This file contains a table of hostnames to IP addresses. It can be used to supplement a DNS server.
sysadmin@localhost:~$ cat /etc/hosts

##### 127.0.0.1 localhost

/etc/resolv.conf	This file contains the IP addresses of the name servers the system should consult in any attempt to resolve names to IP addresses. These servers are often DNS servers. It also can contain additional keywords and values that can affect the resolution process.
sysadmin@localhost:~$ cat /etc/resolv.conf
```

nameserver 127.0.0.11

```text
/etc/nsswitch.conf	This file can be used to modify where hostname lookups occur. It contains a particular entry that describes in what order name resolution sources are consulted.
sysadmin@localhost:~$ cat /etc/nsswitch.conf
```

# /etc/nsswitch.conf
#

Output Omitted...

hosts:          files dns

Output Omitted...
The /etc/hosts file is searched first, the DNS server second:
hosts: files dns
The DNS server would be searched first, local files second:
hosts: dns files
Commands or programs on the system, such as the browser, request a connection with a remote computer by DNS name. Then the system consults various files in a particular order to attempt to resolve that name into a usable IP address.
1. First, the /etc/nsswitch.conf file is consulted:
hosts:          files dns
This line indicates that the system should consult local files first in an attempt to resolve hostnames, which means that the /etc/hosts file will be parsed for a match to the requested name.
2. Second, the system will consult the /etc/hosts file to attempt to resolve the name. If the name matches an entry in /etc/hosts, it is resolved.
It will not failover (or continue) to the DNS option, even if the resolution is inaccurate. This can occur if the entry in /etc/hosts points to a non-assigned IP address.
3. Third, if the local /etc/hosts file doesn’t result in a match, the system will use the configured DNS server entries contained in the /etc/resolv.conf file to attempt to resolve the name.
The /etc/resolv.conf file should contain at least two entries for name servers, such as the example file below:
nameserver 10.0.2.3
nameserver 10.0.2.4
The DNS resolution system will use the first name server for an attempted lookup of the name. If that is unavailable, or a timeout period is reached, the second server will then be queried for the name resolution. If a match is found, it is returned to the system and used for initiating a connection and is also placed in the DNS cache for a configurable time period.

> **Consider This**
>
Two other keywords may appear in the system’s /etc/resolv.conf file. Although these are beyond the scope of this course, they are routinely included in default /etc/resolv.conf files and so we include explanations of these terms below:
domain	Followed by a qualified domain, such as snowblower.example.com, allows the query for the host polaris to be tried both just as the host polaris, or failing that, appending the rest of the domain name to it and hopefully having it resolved by the server as that name (e.g. polaris.snowblower.example.com.).
search	Followed by a set of separate domains which can be queried one after the other hopefully to resolve the name.

### 14.6 Network Tools

There are several commands that you can use to view network information. These tools can also be useful when you are troubleshooting network issues.

#### 14.6.1 The ifconfig Command

The ifconfig command stands for interface configuration and is used to display network configuration information. Not all network settings are covered in this course, but it is important to note from the output below that the IP address of the primary network device eth0 is 192.168.1.2 and that the device is currently active UP:

```text
root@localhost:~# ifconfig
```

eth0      Link encap:Ethernet  HWaddr b6:84:ab:e9:8f:0a
inet addr:192.168.1.2  Bcast:0.0.0.0  Mask:255.255.255.0
inet6 addr: fe80::b484:abff:fee9:8f0a/64 Scope:Link
UP BROADCAST RUNNING MULTICAST  MTU:1500  Metric:1
RX packets:95 errors:0 dropped:4 overruns:0 frame:0
TX packets:9 errors:0 dropped:0 overruns:0 carrier:0
collisions:0 txqueuelen:1000
RX bytes:25306 (25.3 KB)  TX bytes:690 (690.0 B)
lo        Link encap:Local Loopback
inet addr:127.0.0.1  Mask:255.0.0.0
inet6 addr: ::1/128 Scope:Host
UP LOOPBACK RUNNING  MTU:65536  Metric:1
RX packets:6 errors:0 dropped:0 overruns:0 frame:0
TX packets:6 errors:0 dropped:0 overruns:0 carrier:0
collisions:0 txqueuelen:0
RX bytes:460 (460.0 B)  TX bytes:460 (460.0 B)
The lo device is referred to as the loopback device. It is a special network device used by the system when sending network-based data to itself.
The ifconfig command can also be used to modify network settings temporarily. Typically these changes should be permanent, so using the ifconfig command to make such changes is relatively rare.

#### 14.6.2 The ip Command

The ifconfig command is becoming obsolete in some Linux distributions (deprecated) and is being replaced with a form of the ip command, specifically ip addr show.
The ip command differs from ifconfig in several important manners, chiefly that through its increased functionality and set of options, it can almost be a one-stop shop for configuration and control of a system’s networking. The format for the ip command is as follows:
ip [OPTIONS] OBJECT COMMAND
While ifconfig is limited primarily to modification of networking parameters, and displaying the configuration details of networking components, the ip command branches out to do some of the work of several other legacy commands such as route and arp.

> **Note**
>

```text
Linux and Unix commands don’t usually just disappear when they become obsolete; they stick around as a legacy command, sometimes for many years, as the number of scripts that depend on those commands, and the amount of muscle memory amongst system administrators, makes it a good idea to keep them around for compatibility sake.
```

The ip command can initially appear to be a little more verbose than the ifconfig command, but it’s a matter of phrasing and a result of the philosophy behind the operation of the ip command.
In the example below, both the ifconfig command and ip command are used to show all interfaces on the system.

```text
root@localhost:~# ifconfig
```

eth0      Link encap:Ethernet  HWaddr 00:0c:29:71:f0:bb
inet addr:172.16.241.140  Bcast:172.16.241.255  Mask:255.255.255.0
inet6 addr: fe80::20c:29ff:fe71:f0bb/64 Scope:Link
UP BROADCAST RUNNING MULTICAST  MTU:1500  Metric:1
RX packets:8506 errors:0 dropped:0 overruns:0 frame:0
TX packets:1201 errors:0 dropped:0 overruns:0 carrier:0
collisions:0 txqueuelen:1000
RX bytes:8933700 (8.9 MB)  TX bytes:117237 (117.2 KB)

lo        Link encap:Local Loopback
inet addr:127.0.0.1  Mask:255.0.0.0
inet6 addr: ::1/128 Scope:Host
UP LOOPBACK RUNNING  MTU:65536  Metric:1
RX packets:285 errors:0 dropped:0 overruns:0 frame:0
TX packets:285 errors:0 dropped:0 overruns:0 carrier:0
collisions:0 txqueuelen:1
RX bytes:21413 (21.4 KB)  TX bytes:21413 (21.4 KB)

```text
root@localhost:~# ip addr show
```

1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1
link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
inet 127.0.0.1/8 scope host lo
valid_lft forever preferred_lft forever
inet6 ::1/128 scope host
valid_lft forever preferred_lft forever
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc pfifo_fast state UP group default qlen 1000
link/ether 00:0c:29:71:f0:bb brd ff:ff:ff:ff:ff:ff
inet 172.16.241.140/24 brd 172.16.241.255 scope global eth0
valid_lft forever preferred_lft forever
inet6 fe80::20c:29ff:fe71:f0bb/64 scope link
valid_lft forever preferred_lft forever
Both show the type of interface, protocols, hardware and IP addresses, network masks and various other information about each of the active interfaces on the system.

#### 14.6.3 The route Command

Recall that a router (or gateway) is a machine that allows hosts from one network to communicate with another network. To view a table that describes where network packages are sent, use the route command:

```text
root@localhost:~# route
```

Kernel IP routing table
Destination     Gateway         Genmask         Flags Metric Ref    Use Iface

##### 192.168.1.0 * 255.255.255.0 U 0 0 0 eth0

default         192.168.1.1     0.0.0.0        UG     0      0        0 eth0
The first highlighted line in the preceding example indicates that any network packet sent to a machine in the 192.168.0 network is not sent to a gateway machine (the * indicates no gateway). The second highlighted line indicates that all other network packets are sent to the host with the IP address of 192.168.1.1 (the router).
Some users prefer to display this information with numeric data only, by using the -n option to the route command. For example, compare the following and focus on where the previous output displayed the word default:

```text
root@localhost:~# route -n
```

Kernel IP routing table
Destination     Gateway         Genmask         Flags Metric Ref    Use Iface

##### 192.168.1.0 0.0.0.0 255.255.255.0 U 0 0 0 eth0

##### 0.0.0.0 192.168.1.1 0.0.0.0 UG 0 0 0 eth0

The 0.0.0.0 refers to all other machines, and is the same as default.
The route command is becoming obsolete in some Linux distributions (deprecated) and is being replaced with a form of the ip command, specifically ip route or ip route show. Note that the same information highlighted above can also be found using this command:

```text
root@localhost:~# ip route show
```

default via 192.168.1.254 dev eth0 proto static
192.168.1.0/24 dev eth0  proto kernel  scope link  src 192.168.1.2

#### 14.6.4 The ping Command

The ping command can be used to determine if another machine is reachable. If the ping command can send a network package to another machine and receive a response, then you should be able to connect to that machine.
By default, the ping command continues sending packages endlessly. To limit how many pings to send, use the -c option followed by a number indicating how many iterations you desire. The following examples show ping being limited to 4 iterations.
If the ping command is successful, it looks like the following example:

```text
root@localhost:~# ping -c 4 192.168.1.2
```

PING 192.168.1.2 (192.168.1.2) 56(84) bytes of data.

## 64 bytes from 192.168.1.2: icmp_req=1 ttl=64 time=0.051 ms

## 64 bytes from 192.168.1.2: icmp_req=2 ttl=64 time=0.064 ms

## 64 bytes from 192.168.1.2: icmp_req=3 ttl=64 time=0.050 ms

## 64 bytes from 192.168.1.2: icmp_req=4 ttl=64 time=0.043 ms

```text
--- 192.168.1.2 ping statistics ---

## 4 packets transmitted, 4 received, 0% packet loss, time 2999ms

```

rtt min/avg/max/mdev = 0.043/0.052/0.064/0.007 ms
If the ping command fails, a message stating, Destination Host Unreachable displays:

```text
root@localhost:~# ping -c 4 192.168.1.1
```

PING 192.168.1.1 (192.168.1.1) 56(84) bytes of data.
From 192.168.1.2 icmp_seq=1 Destination Host Unreachable
From 192.168.1.2 icmp_seq=2 Destination Host Unreachable
From 192.168.1.2 icmp_seq=3 Destination Host Unreachable
From 192.168.1.2 icmp_seq=4 Destination Host Unreachable

```text
--- 192.168.1.1 ping statistics ---

## 4 packets transmitted, 0 received, +4 errors, 100% packet loss, time 2999ms

```

pipe 4
It is important to note that just because the ping command fails does not mean that the remote system is unreachable. Some administrators configure their machines (and even entire networks!) to not respond to ping requests because a server can be attacked by something called a denial of service attack. In this sort of attack, a server is overwhelmed by a massive number of network packets. By ignoring ping requests, the server is less vulnerable.
As a result, the ping command may be useful for checking the availability of local machines, but not always for machines outside of your own network.

> **Consider This**
>
Many administrators use the ping command with a hostname, and if that fails then use the IP address to see if the fault is in resolving the device’s hostname. Using the hostname first saves time; if that ping command is successful, there is proper name resolution, and the IP address is functioning correctly as well.

#### 14.6.5 The netstat Command

The netstat command is a powerful tool that provides a large amount of network information. It can be used to display information about network connections as well as display the routing table similar to the route command.
For example, to display statistics regarding network traffic, use the -i option to the netstat command:

```text
root@localhost:~# netstat -i
```

Kernel Interface table
Iface   MTU Met   RX-OK RX-ERR RX-DRP RX-OVR    TX-OK TX-ERR TX-DRP TX-OVR Flg
eth0       1500 0       137      0      4 0        12      0      0      0 BMRU
lo        65536 0        18      0      0 0        18      0      0      0 LRU
The most important statistics from the output above are the TX-OK and TX-ERR. A high percentage of TX-ERR may indicate a problem on the network, such as too much network traffic.
To use the netstat command to display routing information, use the -r option:

```text
root@localhost:~# netstat -r
```

Kernel IP routing table
Destination     Gateway         Genmask         Flags   MSS Window  irtt Iface

##### 192.168.1.0 * 255.255.255.0 U 0 0 0 eth0

default         192.168.1.1     0.0.0.0        UG         0 0          0 eth0
The netstat command is also commonly used to display open ports. A port is a unique number that is associated with a service provided by a host. If the port is open, then the service is available for other hosts.
For example, you can log into a host from another host using a service called SSH. The SSH service is assigned port #22. So, if port #22 is open, then the service is available to other hosts.
It is important to note that the host also needs to have the services running itself; this means that the service (in this case the ssh daemon) that allows remote users to log in needs to be started (which it typically is, for most Linux distributions).
To see a list of all currently open ports, use the following command:

```text
root@localhost:~# netstat -tln
```

Active Internet connections (only servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State
tcp        0      0 192.168.1.2:53          0.0.0.0:*               LISTEN
tcp        0      0 127.0.0.1:53            0.0.0.0:*               LISTEN
tcp        0      0 0.0.0.0:22              0.0.0.0:*               LISTEN
tcp        0      0 127.0.0.1:953           0.0.0.0:*               LISTEN
tcp6       0      0 :::53                   :::*                    LISTEN
tcp6       0      0 :::22                  :::*                    LISTEN
tcp6       0      0 ::1:953                 :::*                    LISTEN
As you can see from the output above, port #22 is listening, which means it is open.
In the previous example, -t stands for TCP (recall this protocol from earlier in this chapter), -l stands for listening (which ports are listening) and -n stands for show numbers, not names.
Sometimes showing the names can be more useful. This can be achieved by dropping the -n option:

```text
root@localhost:~# netstat -tl
```

Active Internet connections (only servers)
Proto Recv-Q Send-Q Local Address           Foreign Address          State
tcp        0      0 cserver.example.:domain *:*                     LISTEN
tcp        0      0 localhost:domain        *:*                     LISTEN
tcp        0      0 *:ssh                   *:*                     LISTEN
tcp        0      0 localhost:953           *:*                     LISTEN
tcp6       0      0 [::]:domain             [::]:*                  LISTEN
tcp6       0      0 [::]:ssh                [::]:*                  LISTEN
tcp6       0      0 localhost:953           [::]:*                  LISTEN
On some distributions you may see the following message in the man page of the netstat command:

> **Note**
>
This program is obsolete. Replacement for netstat is ss. Replacement for
netstat -r is ip route. Replacement for netstat -i is ip -s link.
Replacement for netstat -g is ip maddr.
While no further development is being done on the netstat command, it is still an excellent tool for displaying network information. The goal is to eventually replace the netstat command with commands such as the ss and ip commands. However, it is important to realize that this may take some time.

#### 14.6.6 The ss Command

The ss command is designed to show socket statistics and supports all the major packet and socket types. Meant to be a replacement for and to be similar in function to the netstat command, it also shows a lot more information and has more features.
The main reason a user would use the ss command is to view what connections are currently established between their local machine and remote machines, statistics about those connections, etc.
Similar to the netstat command, you can get a great deal of useful information from the ss command just by itself as shown in the example below.

```text
root@localhost:~# ss
```

Netid  State      Recv-Q Send-Q         Local Address:Port                 Peer Address:Port
u_str  ESTAB      0      0                    * 104741                     * 104740
u_str  ESTAB      0      0      /var/run/dbus/system_bus_socket 14623      * 14606
u_str  ESTAB      0      0      /var/run/dbus/system_bus_socket 13582      * 13581
u_str  ESTAB      0      0      /var/run/dbus/system_bus_socket 16243      * 16242
u_str  ESTAB      0      0                    * 16009                      * 16010
u_str  ESTAB      0      0      /var/run/dbus/system_bus_socket 10910      * 10909
u_str  ESTAB      0      0      @/tmp/dbus-LoJW0hGFkV 15706                * 15705
u_str  ESTAB      0      0                    * 24997                      * 24998
u_str  ESTAB      0      0                    * 16242                      * 16243
u_str  ESTAB      0      0              @/tmp/dbus-opsTQoGE 15471          * 15470
The output is very similar to the output of the netstat command with no options. The columns above are:
Netid	The socket type and transport protocol
State	Connected or Unconnected, depending on protocol
Recv-Q	Amount of data queued up for being processed having been received
Send-Q	Amount of data queued up for being sent to another host
Local Address	The address and port of the local host’s portion of the connection
Peer Address	The address and port of the remote host’s portion of the connection
The format of the output of the ss command can change dramatically, given the options specified, such as the use of the -s option, which displays mostly the types of sockets, statistics about their existence and numbers of actual packets sent and received via each socket type, as shown below:

```text
root@localhost:~# ss -s
```

Total: 1000 (kernel 0)
TCP:   7 (estab 0, closed 0, orphaned 0, synrecv 0, timewait 0/0), ports 0

Transport Total     IP        IPv6
*               0         -         -
RAW             0         0         0
UDP             9         6         3
TCP             7         3         4
INET            16        9         7
FRAG            0         0         0

> **Consider This**
>
The ss command typically shows many rows of data, and it can be somewhat daunting to try to find what you want in all that output. Consider sending the output to the less command to make the output more manageable. Pagers allow the user to scroll up and down, do searches and many other useful functions inside the parameters of the less command.
While the ss command offers many different options for gathering and displaying information, the examples above are the most common ones, and anything else would be outside of the scope of the exam’s objectives at this level.

#### 14.6.7 The dig Command

There may be times when you need to test the functionality of the DNS server that your host is using. One way of doing this is to use the dig command, which performs queries on the DNS server to determine if the information needed is available on the server.
In the following example, the dig command is used to determine the IP address of the example.com host:

```text
root@localhost:~# dig example.com
```

; <<>> DiG 9.8.1-P1 <<>> example.com
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 45155
;; flags: qr aa rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 1, ADDITIONAL: 0

;; QUESTION SECTION:
;example.com.                   IN      A

;; ANSWER SECTION:
example.com.            86400   IN      A       192.168.1.2
;; AUTHORITY SECTION:
example.com.            86400   IN      NS      example.com.

;; Query time: 0 msec
;; SERVER: 127.0.0.1#53(127.0.0.1)
;; WHEN: Tue Dec  8 17:54:41 2015
;; MSG SIZE  rcvd: 59
Note that the response included the IP address of 192.168.1.2, meaning that the DNS server has the IP address to hostname translation information in its database.
If the DNS server doesn't have the requested information, it is configured to ask other DNS servers. If none of them have the requested information, an error message displays:

```text
root@localhost:~# dig sample.com
```

; <<>> DiG 9.8.1-P1 <<>> sample.com
;; global options: +cmd
;; connection timed out; no servers could be reached

#### 14.6.8 The host Command

In its simplest form, the host command works with DNS to associate a hostname with an IP address. As used in a previous example, example.com is associated with the IP address of 192.168.1.2:

```text
root@localhost:~# host example.com
```

example.com has address 192.168.1.2
The host command can also be used in reverse if an IP address is known, but the domain name is not.

```text
root@localhost:~# host 192.168.1.2
```

2.1.168.192.in-addr.arpa domain name pointer example.com.
2.1.168.192.in-addr.arpa domain name pointer cserver.example.com.
Other options exist to query the various aspects of a DNS such as a CNAME canonical name -alias:

```text
root@localhost:~# host -t CNAME example.com
```

example.com has no CNAME record
Since many DNS servers store a copy of example.com, SOA Start of Authority records indicate the primary server for the domain:

```text
root@localhost:~# host -t SOA example.com
```

example.com has SOA record example.com. cserver.example.com. 2 604800 86400 2419200 604800
A comprehensive list of DNS information regarding example.com can be found using the -a all option:

```text
root@localhost:~# host -a example.com
```

Trying "example.com"
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 3549
;; flags: qr aa rd ra; QUERY: 1, ANSWER: 3, AUTHORITY: 0, ADDITIONAL: 1

;; QUESTION SECTION:
;example.com.                   IN      ANY

;; ANSWER SECTION:
example.com.            86400   IN      SOA     example.com. cserver.example.com. 2 604800 86400 2419200 604800
example.com.            86400   IN      NS      example.com.
example.com.            86400   IN      A       192.168.1.2

;; ADDITIONAL SECTION:
example.com.            86400   IN      A       192.168.1.2

Received 119 bytes from 127.0.0.1#53 in 0 ms

#### 14.6.9 The ssh Command

The ssh command allows you to connect to another machine across the network, log in and then perform tasks on the remote machine.
If you only provide a machine name or IP address to log into, the ssh command assumes you want to log in using the same username that you are currently logged in as. To use a different username, use the syntax:
username@hostname

```text
root@localhost:~# ssh bob@test
```

The authenticity of host ‘test (127.0.0.1)’ can’t be established.
RSA key fingerprint is c2:0d:ff:27:4c:f8:69:a9:c6:3e:13:da:2f:47:e4:c9.
Are you sure you want to continue connection (yes/no)? yes
Warning: Permanently added ‘test’ (RSA) to the list of known hosts.
bob@test’s password:

```text
bob@test:~$ date
```

Fri Oct   4 16:14:43 CDT 2013
To return back to the local machine, use the exit command:

```text
bob@test:~$ exit
```

logout
Connection to test closed.

```text
root@localhost:~#
```

Warning
Be careful, if you use the exit command too many times, you will close the terminal window that you are working in!

##### 14.6.9.1 RSA Key Fingerprint

When using the ssh command, the first prompt asks you to verify the identity of the machine you are logging into. In most cases, you are going to want to answer yes. While you can check with the administrator of the remote machine to make sure that the RSA key fingerprint is correct, this isn't the purpose of this query. It is designed for future login attempts.
After you answer yes, the RSA key fingerprint of the remote machine is stored on your local system. When you attempt to ssh to this same machine in the future, the RSA key fingerprint provided by the remote machine is compared to the copy stored on the local machine. If they match, then the username prompt appears. If they don't match, an error like the following displays:

```text
sysadmin@localhost:~$ ssh bob@test
```

@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@   WARNING: REMOTE HOST IDENTIFICATION HAS CHANGED!   @
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
IT IS POSSIBLE THAT SOMEONE IS DOING SOMETHING NASTY!
Someone could be eavesdropping on you right now (man-in-the-middle attack)!
It is also possible that the RSA host key has just been changed.
The fingerprint for the RSA key sent by the remote host is
c2:0d:ff:27:4c:f8:69:a9:c6:3e:13:da:2f:47:e4:c9.
Please contact your system administrator.
Add correct host key in /home/sysadmin/.ssh/known_hosts to get rid of this message.
Offending key in /home/sysadmin/.ssh/known_hosts:1
RSA host key for test has changed and you have requested strict checking.
Host key verification failed.
This error could indicate that a rogue host has replaced the correct host. Check with the administrator of the remote system. If the system were recently reinstalled, it would have a new RSA key, and that would be causing this error.
In the event that this error message is due to a remote machine reinstall, you can remove the ~/.ssh/known_hosts file from your local system (or just remove the entry for that one machine) and try to connect again:

```text
sysadmin@localhost:~$ cat ~/.ssh/known_hosts
```

test ssh-rsa AAAAB3NzaC1yc2EAAAAmIwAAAQEAklOUpkDHrfHY17SbrmTIp/RZ0V4DTxgq9wzd+ohy006SWDSGPA+nafzlHDPOW7vdI4mZ5ew18KL4JW9jbhUFrviQzM7xlELEVf4h9lFX5QVkbPppSrg0cda3Pbv7kOdJ/MTyBlWXFCRH+Cv3FXRitBqxiX1nKhXpHAZsMciLq8V6RjsNAQwdsdMFvSlVK/7BA
t5FaiKoAfncM1Q8x3+2V0Ww71/eIFmb1zuUFljHYTprrX88XypNDvjYNby6vw/Pb0rwprz/Tn
mZAW3UX+PnTPI89ZPmNBLuxyrD2cE86Z/il8b+gw3r3+1nJotmIkjn2so1d01QraTlMqVSsbx
NrRFi9wrf+ghw==

```text
sysadmin@localhost:~$ rm ~/.ssh/known_hosts
sysadmin@localhost:~$ ssh bob@test
```

The authenticity of host ‘test (127.0.0.1)’ can’t be established.
RSA key fingerprint is c2:0d:ff:27:4c:f8:69:a9:c6:3e:13:da:2f:47:e4:c9.
Are you sure you want to continue connection (yes/no)? yes
Warning: Permanently added ‘test’ (RSA) to the list of known hosts.
bob@test’s password:
Last login: Fri Oct   4 16:14:39 CDT 2013  from localhost

### 17.1 Introduction

File ownership is critical for file security. Every file has a user owner and a group owner.
This chapter focuses on how to specify the user and group ownership of a file. In addition, the concept of file and directory permissions is explored, including how to change the permissions on files and directories. Default permissions are the permissions given to files and directories when they are initially created.

### 17.2 File Ownership

By default, users own the files that they create. While this ownership can be changed, this function requires administrative privileges. Although most commands usually show the user owner as a name, the operating system is associating the user ownership with the UID for that username.
Every file also has a group owner. By default, the primary group of the user who creates the file is the group owner of any new files. Users are allowed to change the group owner of files they own to any group that they belong to. Similar to user ownership, the association of a file with a group is not done internally by the operating system by name, but by the GID of the group.
Since ownership is determined by the UID and GID associated with a file, changing the UID of a user (or deleting the user) has the effect of making a file that was originally owned by that user have no real user owner. When there is no UID in the /etc/passwd file that matches the UID of the owner of the file, then the UID (the number) is displayed as the user owner of the file instead of the username (which no longer exists). The same occurs for groups.
The id command can be useful for verifying which user account you are using and which groups you have available to use. By viewing the output of this command, you can see the user's identity information expressed both as a number and as a name.
The output of the id command displays the UID and user account name of the current user followed by the GID and group name of the primary group and the GIDs and group names of all group memberships:

```text
sysadmin@localhost:~$ id
```

uid=1001(sysadmin) gid=1001(sysadmin) groups=1001(sysadmin),4(adm),27(sudo),1005(research),1006(development)
The above example shows the user has a UID of 1001 for the user account sysadmin. It also shows that the primary group for this user has a GID of 1001 for the group sysadmin.
Because the user account and primary group account have the same numeric identifier and name, this indicates that this user is in a User Private Group (UPG). In addition, the user in this example belongs to four supplemental groups: the adm group with a GID of 4, the sudo group with a GID of 27, the research group with a GID of 1005 and the development group with a GID of 1006.
When a file is created, it belongs to the current user and their current primary group. If the user from the previous example executes the touch command to create a file, then the user owner of the file is the sysadmin user, and the group owner is the sysadmin group:

```text
sysadmin@localhost:~$ touch /tmp/filetest1
```

The file ownership can be confirmed using the long listing -l option of the ls command.

```text
sysadmin@localhost:~$ ls -l /tmp/filetest1
-rw-rw-r--. 1 sysadmin sysadmin 0 Oct 21 10:18 /tmp/filetest1
```

File ownership also applies to hidden files in the system. Hidden files, which begin with the period . character are listed using the -a option of the ls command. The first two hidden files listed are the current . and parent .. directories respectively. The ownership of all files and subdirectories within the current directory can be listed using the ls -la command.

```text
sysadmin@localhost:~$ ls -la
```

total 60
drwxr-xr-x 1 sysadmin sysadmin 4096 Nov  3 22:29 .
drwxr-xr-x 1 root     root     4096 Mar 14  2016 ..

```text
-rw-r--r-- 1 sysadmin sysadmin  220 Apr  3  2012 .bash_logout
-rw-r--r-- 1 sysadmin sysadmin 3768 Mar 14  2016 .bashrc
```

drwx------ 2 sysadmin sysadmin 4096 Nov  3 22:29 .cache

```text
-rw-r--r-- 1 sysadmin sysadmin  675 Apr  3  2012 .profile
-rw-r--r-- 1 sysadmin sysadmin   74 Mar 14  2016 .selected_editor
```

drwxr-xr-x 2 sysadmin sysadmin 4096 Mar 14  2016 Desktop
drwxr-xr-x 2 sysadmin sysadmin 4096 Mar 14  2016 Documents
drwxr-xr-x 2 sysadmin sysadmin 4096 Mar 14  2016 Downloads
drwxr-xr-x 2 sysadmin sysadmin 4096 Mar 14  2016 Music
drwxr-xr-x 2 sysadmin sysadmin 4096 Mar 14  2016 Pictures
drwxr-xr-x 2 sysadmin sysadmin 4096 Mar 14  2016 Public
drwxr-xr-x 2 sysadmin sysadmin 4096 Mar 14  2016 Templates
drwxr-xr-x 2 sysadmin sysadmin 4096 Mar 14  2016 Videos

> **Consider This**
>
The output of the ls -l command includes multiple pieces of information that are relevant to this chapter including:
1. Permissions

```text
-rw-rw-r--. 1 sysadmin sysadmin 0 Oct 21 10:18 /tmp/filetest1
2. User Owner
-rw-rw-r--. 1 sysadmin sysadmin 0 Oct 21 10:18 /tmp/filetest1
3. Group Owner
-rw-rw-r--. 1 sysadmin sysadmin 0 Oct 21 10:18 /tmp/filetest1

### 17.3 Changing Groups

```

If you know that the file you are about to create should belong to a group different from your current primary group, then you can use the newgrp command to change your current primary group.
newgrp group_name
The id command lists your identity information, including your group memberships. If you are only interested in knowing what groups you belong to, then you can execute the groups command:

```text
sysadmin@localhost:~$ groups
```

sysadmin adm sudo research development
The output of the groups command may not be as detailed as the output of the id command, but if all you need to know is what groups you can switch to by using the newgrp command, then the groups command provides the information that you need. The id command output does show your current primary group, so it is useful for verifying that the newgrp command succeeded.
For example, if the sysadmin user was planning on having a file owned by the group research, but that wasn't the user's primary group, then the user could use the newgrp command and then verify the correct primary group with the id command before creating the new file:

```text
sysadmin@localhost:~$ id
```

uid=1001(sysadmin) gid=1001(sysadmin) groups=1001(sysadmin),4(adm),27(sudo),1005(research),1006(development)

```text
sysadmin@localhost:~$ newgrp research
sysadmin@localhost:~$ id
```

uid=1001(sysadmin) gid=1005(research) groups=1005(research),4(adm),27(sudo),1001(sysadmin),1006(development)
According to the output of the previous commands, initially the user's GID is 1001 for the sysadmin user, then the newgrp command is executed, and the user's primary GID becomes 1005, the research group. After these commands were executed, if the user were to create another file and view its details, the new file would be owned by the research group:

```text
sysadmin@localhost:~$ touch /tmp/filetest2
sysadmin@localhost:~$ ls -l /tmp/filetest2
-rw-r--r--. 1 sysadmin research 0 Oct 21 10:53 /tmp/filetest2
```

The newgrp command opens a new shell; as long as the user stays in that shell, the primary group won't change. To switch the primary group back to the original, the user can leave the new shell by running the exit command. For example:

```text
sysadmin@localhost:~$ id
```

uid=1001(sysadmin) gid=1005(research) groups=1005(research),4(adm),27(sudo),1001
(sysadmin),1006(development)

```text
sysadmin@localhost:~$ exit
```

exit

```text
sysadmin@localhost:~$ id
```

uid=1001(sysadmin) gid=1001(sysadmin) groups=1001(sysadmin),4(adm),27(sudo),1005(research),1006(development)

> **Consider This**
>
Administrative privileges are required to change the primary group of the user permanently. The root user would execute the following command:
usermod -g groupname username

### 17.4 Changing Group Ownership

To change the group owner of an existing file the chgrp command can be used.
chgrp group_name file
As the root user, the chgrp command can be used to change the group owner of any file to any group. As a user without administrative privileges, the chgrp command can only be used to change the group owner of a file to a group that the user is already a member of:

```text
sysadmin@localhost:~$ touch sample
sysadmin@localhost:~$ ls -l sample
-rw-rw-r-- 1 sysadmin sysadmin 0 Oct 23 22:12 sample‌⁠​​⁠​
sysadmin@localhost:~$ chgrp research sample
sysadmin@localhost:~$ ls -l sample
-rw-rw-r--. 1 sysadmin research 0 Oct 23 22:12 sample‌⁠​​⁠​
```

If a user attempts to modify the group ownership of a file that the user doesn't own, they receive an error message:

```text
sysadmin@localhost:~$ chgrp development /etc/passwd
```

chgrp: changing group of '/etc/passwd': Operation not permitted
To change the group ownership of all of the files of a directory structure, use the recursive -R option to the chgrp command. For example, the command in the following example would change the group ownership of the test_dir directory and all files and subdirectories of the test_dir directory.

```text
sysadmin@localhost:~$ chgrp -R development test_dir

> **Consider This**
>
```

While you can view the ownership of a file with the -l option to the ls command, the system provides another command that is useful when viewing ownership and file permissions: the stat command. The stat command displays more detailed information about a file, including providing the group ownership both by group name and GID number:

```text
sysadmin@localhost:~$ stat /tmp/filetest1
```

File: `/tmp/filetest1'
Size: 0               Blocks: 0          IO Block: 4096   regular empty file
Device: fd00h/64768d    Inode: 31477       Links: 1
Access: (0664/-rw-rw-r--)  Uid: ( 1001/sysadmin)   Gid: ( 1001/sysadmin)
Access: 2013-10-21 10:18:02.809118163 -0700
Modify: 2013-10-21 10:18:02.809118163 -0700
Change: 2013-10-21 10:18:02.809118163 -0700

### 17.4 Changing Group Ownership

To change the group owner of an existing file the chgrp command can be used.
chgrp group_name file
As the root user, the chgrp command can be used to change the group owner of any file to any group. As a user without administrative privileges, the chgrp command can only be used to change the group owner of a file to a group that the user is already a member of:

```text
sysadmin@localhost:~$ touch sample
sysadmin@localhost:~$ ls -l sample
-rw-rw-r-- 1 sysadmin sysadmin 0 Oct 23 22:12 sample‌⁠​​⁠​
sysadmin@localhost:~$ chgrp research sample
sysadmin@localhost:~$ ls -l sample
-rw-rw-r--. 1 sysadmin research 0 Oct 23 22:12 sample‌⁠​​⁠​
```

If a user attempts to modify the group ownership of a file that the user doesn't own, they receive an error message:

```text
sysadmin@localhost:~$ chgrp development /etc/passwd
```

chgrp: changing group of '/etc/passwd': Operation not permitted
To change the group ownership of all of the files of a directory structure, use the recursive -R option to the chgrp command. For example, the command in the following example would change the group ownership of the test_dir directory and all files and subdirectories of the test_dir directory.

```text
sysadmin@localhost:~$ chgrp -R development test_dir

> **Consider This**
>
```

While you can view the ownership of a file with the -l option to the ls command, the system provides another command that is useful when viewing ownership and file permissions: the stat command. The stat command displays more detailed information about a file, including providing the group ownership both by group name and GID number:

```text
sysadmin@localhost:~$ stat /tmp/filetest1
```

File: `/tmp/filetest1'
Size: 0               Blocks: 0          IO Block: 4096   regular empty file
Device: fd00h/64768d    Inode: 31477       Links: 1
Access: (0664/-rw-rw-r--)  Uid: ( 1001/sysadmin)   Gid: ( 1001/sysadmin)
Access: 2013-10-21 10:18:02.809118163 -0700
Modify: 2013-10-21 10:18:02.809118163 -0700
Change: 2013-10-21 10:18:02.809118163 -0700

### 17.6 Permissions

The output of the ls -l command displays ten characters at the beginning of each line. These characters indicate the type of file and the permissions of the file. For example, consider the output of the following command:

```text
root@localhost:~# ls -l /etc/passwd
-rw-r--r--. 1 root root 4135 May 27 21:08 /etc/passwd
```

File Type
The first character of each line indicates the type of file:

```text
-rw-r--r-- 1 root root 4135 May 27 21:08 /etc/passwd
```

The following table describes the possible values for the file type:
Character	Type of the File

```text
-	A regular file, which may be empty, or contain text or binary data.
```

d	A directory file, which contains the names of other files and links to them.
l	A symbolic link is a file name that refers (points) to another file.
b	A block file is one that relates to a block hardware device where data is read in blocks of data.
c	A character file is one that relates to a character hardware device where data is read one byte at a time.
p	A pipe file works similar to the pipe symbol, allowing for the output of one process to communicate to another process through the pipe file, where the output of the one process is used as input for the other process.
s	A socket file allows two processes to communicate, where both processes are allowed to either send or receive data.

> **Consider This**
>
Although all the file types are listed in the table above, typically you don’t encounter anything but regular, directory and link files unless you explore the /dev directory.
Permission Groups
The next nine characters demonstrate the permissions of the file.

```text
-rw-r--r-- 1 root root 4135 May 27 21:08 /etc/passwd
```

The permissions set on these files determine the level of access that a user has on the file. When a user runs a program and the program accesses a file, then the permissions are checked to determine whether the user has the correct access rights to the file.
The permissions are grouped into three different roles, representing the different users that may try to access the file.
If you aren't the owner and you're not a member of the file/directory group, then your permissions would be others.
User Owner

```text
-rw-r--r-- 1 root root 4135 May 27 21:08 /etc/passwd
```

Characters 2-4 indicate the permissions for the user that owns the file. If you are the owner of the file, then only the user owner permissions are used to determine access to that file.
Group Owner

```text
-rw-r--r-- 1 root root 4135 May 27 21:08 /etc/passwd
```

Characters 5-7 indicate the permissions for the group that owns the file. If you are not the owner but are a member of the group that owns the file, then only group owner permissions are used to determine access to that file.
Other Permissions

```text
-rw-r--r-- 1 root root 4135 May 27 21:08 /etc/passwd
```

Characters 8-10 indicate the permissions for others or what is sometimes referred to as the world's permissions. This group includes all users who are not the file owner or a member of the file's group.
Permission Types
Each group is attributed three basic types of permissions: read, write, and execute.
User Owner 	Group Owner 	Other
Read	Write	Execute
r	w	x
Read	Write
Execute	r	w
x		Read
Write	Execute	r
w	x
The permissions themselves are deceptively simple and have a different meaning depending on whether they are applied to a file or a directory.	Read
The first character of each group represents the read permission. There is an r character if the group has the read permission, or a - character if the group does not.	    • On a file, this allows processes to read the contents of the file, meaning the contents can be viewed and copied. 	    • On a directory, file names in the directory can be listed, but other details are not available.
Write
The second character of each group represents the write permission. There is a w character if the group has the write permission, or a - character if the group does not.
- A file can be written to by the process, so changes to a file can be saved. Note that w permission really requires r permission on the file to work correctly.
- On a directory, files can be added to or removed from the directory. Note that w permission requires x permission on the directory to work correctly.
Execute
The third character of each group represents the execute permission. There is an x character if the group has the execute permission, or a - character if the group does not.
- A file can be executed or run as a process.
- On a directory, the user can use the cd command to "get into" the directory and use the directory in a pathname to access files and, potentially, subdirectories under this directory.

### 17.7 Understanding Permissions

The descriptions of the permission types can be handy, but just themselves, they don't provide a clear description of how permissions work. To better understand how permissions work, consider the following scenarios.
To understand these scenarios, you should first understand the following diagram:
drwxr-xr-x. 17 root root 4096 23:38 /
drwxr-xr-x. 10 root root 128  03:38 /data

```text
-rwxr-xr--.  1 bob  bob  100  21:08 /data/abc.txt
```

The relevant information is highlighted. The first line represents the / directory, with a user owner of root, a group owner of root and permissions of rwxr-xr-x. The second line represents the /data directory, a directory that is under the / directory. The third line represents the abc.txt file, which is stored in the /data directory.

### 17.8 Changing Permissions

The chmod (change mode) command is used to change permissions on files and directories. There are two techniques that can be used with this command: symbolic and numeric. Both techniques use the following basic syntax:
chmod new_permission file_name
Important
To change a file's permissions, you either need to own the file or log in as the root user.
The following examples will use a sample file:

```text
root@localhost:~# touch abc.txt
root@localhost:~# ls -l abc.txt
-rw-r--r-- 1 root root 0 Dec 19 18:58 abc.txt

### 17.9 Default Permissions

```

The umask command is a feature that is used to determine default permissions that are set when a file or directory is created. Default permissions are determined when the umask value is subtracted from the maximum allowable default permissions. The maximum default permissions are different for files and directories:
file	rw-rw-rw-
directories	rwxrwxrwx
The permissions that are initially set on a file when it is created cannot exceed rw-rw-rw-. To have the execute permission set on a file, you first need to create the file and then change the permissions.
The umask command can be used to display the current umask value:

```text
sysadmin@localhost:~$ umask
```

0002
A breakdown of the output:
- The first 0 indicates that the umask is given as an octal number.
- The second 0 indicates which permissions to subtract from the default user owner's permissions.
- The third 0 indicates which permissions to subtract from the default group owner's permissions.
- The last number 2 indicates which permissions to subtract from the default other's permissions.
Note that different users may have different umasks. Typically the root user has a more restrictive umask than normal user accounts:

```text
root@localhost:~# umask
```

0022
To understand how umask works, assume that the umask of a file is set to 027 and consider the following:
File Default	666
Umask	-027
Result	640
The 027 umask means that new files would receive 640 or rw-r----- permissions by default, as demonstrated below:

```text
sysadmin@localhost:~$ umask 027
sysadmin@localhost:~$ touch sample
sysadmin@localhost:~$ ls -l sample
-rw-r-----. 1 sysadmin sysadmin 0 Oct 28 20:14 sample
```

Because the default permissions for directories are different than for files, a umask of 027 would result in different initial permissions on new directories:
Directory Default	777
Umask	-027
Result	750
The 027 umask means that directories files would receive 750 or rwxr-x--- permissions by default, as demonstrated below:

```text
sysadmin@localhost:~$ umask 027
sysadmin@localhost:~$ mkdir test-dir
sysadmin@localhost:~$ ls -ld test-dir
```

drwxr-x---. 1 sysadmin sysadmin 4096 Oct 28 20:25 test-dir
The new umask is only applied to file and directories created during that session. When a new shell is started, the default umask will again be in effect.
Permanently changing a user's umask requires modifying the .bashrc file located in that user's home directory.

### 18.1 Introduction

In most circumstances, the basic Linux permissions, read, write, and execute, are enough to accommodate the security needs of individual users or organizations.
However, when multiple users need to work routinely on the same directories and files, these permissions may not be enough. The special permissions setuid, setgid and the sticky bit are designed to address these concerns.

### 18.2 Setuid

When the setuid permission is set on an executable binary file (a program) the binary file is run as the owner of the file, not as the user who executed it. This permission is set on a handful of system utilities so that they can be run by normal users, but executed with the permissions of root, providing access to system files that the normal user doesn't normally have access to.
Consider the following scenario in which the user sysadmin attempts to view the contents of the /etc/shadow file:

```text
sysadmin@localhost:~$ more /etc/shadow
```

/etc/shadow: Permission denied

```text
sysadmin@localhost:~$ ls -l /etc/shadow
-rw-r-----. 1 root root 5195 Oct 21 19:57 /etc/shadow
```

The permissions on /etc/shadow do not allow normal users to view (or modify) the file. Since the file is owned by the root user, the administrator can temporarily modify the permissions to view or modify this file.
Now consider the passwd command. When this command runs, it modifies the /etc/shadow file, which seems impossible because other commands that the sysadmin user runs that try to access this file fail. So, why can the sysadmin user modify the /etc/shadow file while running the passwd command when normally this user has no access to the file?
The passwd command has the special setuid permission set. When the passwd command is run, and the command accesses the /etc/shadow file, the system acts as if the user accessing the file is the owner of the passwd command (the root user), not the user who is running the command.
You can see this permission set by running the ls -l command:

```text
sysadmin@localhost:~$ ls -l /usr/bin/passwd
-rwsr-xr-x 1 root root 31768 Jan 28 2010 /usr/bin/passwd
```

Notice the output of the ls command above; the setuid permission is represented by the s in the owner permissions where the execute permission would normally be represented. A lowercase s means that both the setuid and execute permission are set, while an uppercase S means that only setuid and not the user execute permission is set.
Like the read, write and execute permissions, special permissions can be set with the chmod command, using either the symbolic and octal methods.
To add the setuid permission symbolically, run:
chmod u+s file
To add the setuid permission numerically, add 4000 to the file's existing permissions (assume the file originally had 775 for its permission in the following example):
chmod 4775 file
To remove the setuid permission symbolically, run:
chmod u-s file
To remove the setuid permission numerically, subtract 4000 from the file's existing permissions:
chmod 0775 file
Previously, we set permission with the octal method using three-digit codes. When a three-digit code is provided, the chmod command assumes that the first digit before the three-digit code is 0. Only when four digits are specified is a special permission set.
If three digits are specified when changing the permission on a file that already has a special permission set, the first digit will be set to 0, and the special permission will be removed from the file.

### 18.3 Setgid

The setgid permission is similar to setuid, but it makes use of the group owner permissions. There are two forms of setgid permissions: setgid on a file and setgid on a directory. The behavior of setgid depends on whether it is set on a file or directory.

#### 18.3.1 Setgid on Files

The setgid permission on a file is very similar to setuid; it allows a user to run an executable binary file in a manner that provides them additional (temporary) group access. The system allows the user running the command to effectively belong to the group that owns the file, but only in the setgid program.
A good example of the setgid permission on an executable file is the /usr/bin/wall command. Notice the permissions for this file as well as the group owner:

```text
sysadmin@localhost:~$ ls -l /usr/bin/wall
-rwxr-sr-x 1 root tty 30800 May 16  2018 /usr/bin/wall
```

You can see that this file is setgid by the presence of the s in the group's execute position. Due to this executable being owned by the tty group, when a user executes this command, the command is able to access files that are group owned by the tty group.
This access is important because the /usr/bin/wall command sends messages to terminals, which is accomplished by writing data to files like the following:

```text
sysadmin@localhost:~$ ls -l /dev/tty?
```

crw--w----. 1 root tty  4, 0 Mar 29  2013 /dev/tty0
crw--w----. 1 root tty  4, 1 Oct 21 19:57 /dev/tty1
Note that the tty group has write permission on the files above while users who are not in the tty group ("others") have no permissions on these files. Without the setgid permission, the /usr/bin/wall command would fail.

#### 18.3.2 Setgid on Directories

When set on a directory, the setgid permission causes files created in the directory to be owned by the group that owns the directory automatically. This behavior is contrary to how new file group ownership would normally function, as by default new files are group owned by the primary group of the user who created the file.
In addition, any directories created within a directory with the setgid permission set are not only owned by the group that owns the setgid directory, but the new directory automatically has setgid set on it as well. In other words, if a directory is setgid, then any directories created within that directory inherit the setgid permission.
By default when the ls command is executed on a directory, it outputs information on the files contained within the directory. To view information about the directory itself add the -d option. Used with the -l option, it can be used to determine if the setgid permission is set. The following example shows that the /tmp/data directory has the setgid permission set and that it is owned by the demo group.

```text
sysadmin@localhost:~$ ls -ld /tmp/data
```

drwxrwsrwx. 2 root demo 4096 Oct 30 23:20 /tmp/data
In a long listing, the setgid permission is represented by an s in the group execute position. A lowercase s means that both setgid and group execute permissions are set:
drwxrwsrwx. 2 root demo 4096 Oct 30 23:20 /tmp/data
An uppercase S means that only setgid and not group execute permission is set. If you see an uppercase S in the group execute position of the permissions, then it indicates that although the setgid permission is set, it is not really in effect because the group lacks the execute permission to use it:
drwxrwSr-x. 2 root root 5036 Oct 30 23:22 /tmp/data2
Typically files created by the user sysadmin are owned by their primary group, also called sysadmin.

```text
sysadmin@localhost:~$ id
```

uid=500(sysadmin) gid=500(sysadmin)
groups=500(sysadmin),10001(research),10002(development)
context=unconfined_u:unconfined_r:unconfined_t:s0-s0:c0.c1023
The UID and GID information in the example above may differ from the output in our virtual environment.
However, if the user sysadmin creates a file in the /tmp/data directory, the setgid directory from the preceding example, the group ownership of the file isn't the sysadmin group, but rather the group that owns the directory demo:

```text
sysadmin@localhost:~$  touch /tmp/data/file.txt
sysadmin@localhost:~$  ls -ld /tmp/data/file.txt
-rw-rw-r--. 1 bob demo 0 Oct 30 23:21 /tmp/data/file.txt
```

Why would an administrator want to set up a setgid directory? First, consider the following user accounts:
- The user bob is a member of the payroll group.
- The user sue is a member of the staff group.
- The user tim is a member of the acct group.
In this scenario, these three users need to work on a joint project. They approach the administrator to ask for a shared directory in which they can work together, but that no one else can access their files. The administrator does the following:
1. Creates a new group called team.
2. Adds bob, sue, and tim to the team group.
3. Makes a new directory called /home/team.
4. Makes the group owner of the /home/team directory be the team group.
5. Gives the /home/team directory the following permissions: rwxrwx---
As a result, bob, sue, and tim can access the /home/team directory and add files. However, there is a potential problem: when bob creates a file in the /home/team directory, the new file is owned by his primary group:

```text
-rw-r-----. 1 bob payroll 100 Oct 30 23:21 /home/team/file.txt
```

Unfortunately, while sue and tim can access the /home/team directory, they can't do anything with bob's file. Their permissions for that file are the others permissions (---).
If the administrator sets the setgid permission to the /home/team directory, then when bob creates a file, it is owned the team group:

```text
-rw-r-----. 1 bob team 100 Oct 30 23:21 /home/team/file.txt
```

As a result, sue and tim would have access to the file through the group owner permissions (r--).
Certainly, bob could change the group ownership or the others permissions after creating the file, but that would become tedious if there were many new files being created. The setgid permission makes it easier for this situation.

#### 18.3.3 Setting Setgid

Use the following syntax to add the setgid permission symbolically:
chmod g+s <file|directory>
To add the setgid permission numerically, add 2000 to the file's existing permissions (assume in the following example that the directory originally had 775 for its permissions):
chmod 2775 <file|directory>
To remove the setgid permission symbolically, run:
chmod g-s <file|directory>
To remove the setgid permission numerically, subtract 2000 from the file's existing permissions:
chmod 0775 <file|directory>

### 18.4 Sticky Bit

The sticky bit permission is used to prevent other users from deleting files that they do not own in a shared directory. Recall that any user with write permission on a directory can create files in that directory, as well as delete any file in the directory, even if they do not own the file!
The sticky bit permission allows for files to be shared with other users, by changing write permission on the directory so that users can still add and delete files in the directory, but files can only be deleted by the owner of the file or the root user.
A good example of the use of sticky bit directories would be the /tmp and /var/tmp directories. These directories are designed as locations where any user can create a temporary file.
Because these directories are intended to be writable by all users, they are configured to use the sticky bit. Without this special permission, users would be able to delete any files in this directory, including those that belong to other users.
The output of the ls -l command displays the sticky bit by a t character in the execute bit of the others permission group:

```text
sysadmin@localhost:~$ ls -ld /tmp
```

drwxrwxrwt 1 root root 4096 Mar 14  2016 /tmp
A lowercase t means that both the sticky bit and execute permissions are set for others. An uppercase T means that only the sticky bit permission is set.
While the capital S indicated a problem with the setuid or setgid permissions, a capital T does not necessarily indicate a problem, as long as the group owner still has the execute permission.
To set the sticky bit permission symbolically, execute a command like the following:
chmod o+t <directory>
To set the sticky bit permission numerically, add 1000 to the directory's existing permissions (assume the directory in the following example originally had 775 for its permissions):
chmod 1775 <file|directory>
To remove the sticky permission symbolically, run:
chmod o-t <directory>
‌⁠​​⁠​To remove the sticky bit permission numerically, subtract 1000 from the directory's existing permissions:
chmod 0775 <directory>

### 18.5 Links

Consider a scenario where there is a file deeply buried in the file system called:
/usr/share/doc/superbigsoftwarepackage/data/2013/october/tenth/valuable-information.txt
Another user routinely updates this file, and you need to access it regularly. The long file name is a not an ideal choice for you to type, but the file must reside in this location. It is also updated frequently, so you can't simply make a copy of the file.
In a situation like this, links come in handy. You can create a file that is linked to the one that is deeply buried. This new file could be placed in the home directory or any other convenient location. When you access the linked file, it accesses the contents of the valuable-information.txt file.
Each linking method, hard and symbolic, results in the same overall access, but uses different techniques. There are pros and cons to each method, so knowing both techniques and when to use them is important.

#### 18.5.1 Creating Hard Links

To understand hard links, it is helpful to understand a little bit about how the file system keeps track of files. For every file created, there is a block of data on the file system that stores the metadata of the file. Metadata includes information about the file like the permissions, ownership, and timestamps. Metadata does not include the file name or the contents of the file, but it does include just about all other information about the file.
This metadata is called the file's inode table. The inode table also includes pointers to the other blocks on the file system called data blocks where the data is stored.
Every file on a partition has a unique identification number called an inode number. The ls -i command displays the inode number of a file.

```text
sysadmin@localhost:~$ ls -i /tmp/file.txt

## 215220874 /tmp/file.txt

```

Like users and groups, what defines a file is not its name, but rather the number it has been assigned. The inode table does not include the file name. For each file, there is also an entry that is stored in a directory's data area (data block) that includes an association between an inode number and a file name.
In the data block for the /etc directory, there would be a list of all of the files in this directory and their corresponding inode number. For example:
File Name	Inode Number
passwd	123
shadow	175
group	144
gshadow	897
When you attempt to access the /etc/passwd file, the system uses this table to translate the file name into an inode number. It then retrieves the file data by looking at the information in the inode table for the file.
Hard links are two file names that point to the same inode. For example, consider the following directory entries:
File Name	Inode Number
passwd	123
mypasswd	123
shadow	175
group	144
gshadow	897
Because both the passwd and mypasswd file have the same inode number, they essentially are the same file. You can access the file data using either file name.
When you execute the ls -li command, the number that appears for each file between the permissions and the user owner is the link count number:

```text
sysadmin@localhost:~$ echo data > file.original
sysadmin@localhost:~$ ls -li file.*

## 278772 -rw-rw-r--. 1 sysadmin sysadmin 5 Oct 25 15:42 file.original

```

The link count number indicates how many hard links have been created. When the number is a value of one, then the file has only one name linked to the inode.
To create hard links, the ln command is used with two arguments. The first argument is an existing file name to link to, called a target, and the second argument is the new file name to link to the target.
ln target link_name
When the ln command is used to create a hard link, the link count number increases by one for each additional filename:

```text
sysadmin@localhost:~$ ln file.original file.hard.1
sysadmin@localhost:~$ ls -li file.*

## 278772 -rw-rw-r--. 2 sysadmin sysadmin 5 Oct 25 15:53 file.hard.1

## 278772 -rw-rw-r--. 2 sysadmin sysadmin 5 Oct 25 15:53 file.original

#### 18.5.2 Creating Symbolic Links

```

A symbolic link, also called a soft link, is simply a file that points to another file. There are several symbolic links already on the system, including several in the /etc directory:

```text
sysadmin@localhost:~$ ls -l /etc/grub.conf
```

lrwxrwxrwx. 1 root root 22 Feb 15  2011 /etc/grub.conf -> ../boot/grub/grub.conf
In the previous example, the file /etc/grub.conf "points to" the ../boot/grub/grub.conf file. So, if you were to attempt to view the contents of the /etc/grub.conf file, it would follow the pointer and show you the contents of the ../boot/grub/grub.conf file.
To create a symbolic link, use the -s option with the ln command:
ln -s target link_name

```text
sysadmin@localhost:~$  ln -s /etc/passwd mypasswd
sysadmin@localhost:~$  ls -l mypasswd
```

lrwxrwxrwx. 1 sysadmin sysadmin 11 Oct 31 13:17 mypasswd -> /etc/passwd

> **Consider This**
>
Notice that the first bit of the ls -l output is the l character, indicating that the file type is a link.

#### 18.5.3 Comparing Hard and Symbolic Links

While hard and symbolic links have the same result, the different techniques produce different advantages and disadvantages. In fact, the advantage of one technique compensates for a disadvantage of the other technique.
Advantage: Hard links don’t have a single point of failure.
One of the benefits of using hard links is that every file name for the file content is equivalent. If you have five files hard linked together, then deleting any four of these files would not result in deleting the actual file contents.
Recall that a file is associated with a unique inode number. As long as one of the hard linked files remains, then that inode number still exists, and the file data still exists.
Symbolic links, however, have a single point of failure: the original file. Consider the following example in which access to the data fails if the original file is deleted. The mytest.txt file is a symbolic link to the text.txt file:

```text
sysadmin@localhost:~$ ls -l mytest.txt
```

lrwxrwxrwx. 1 sysadmin sysadmin 8 Oct 31 13:29 mytest.txt -> test.txt

```text
sysadmin@localhost:~$ more test.txt
```

hi there

```text
sysadmin@localhost:~$ more mytest.txt
```

hi there
If the original file, the test.txt file is removed, then any files linked to it, including the mytest.txt file, fail:

```text
sysadmin@localhost:~$ rm test.txt
sysadmin@localhost:~$ more mytest.txt
```

mytest.txt: No such file or directory

```text
sysadmin@localhost:~$ ls -l mytest.txt
```

lrwxrwxrwx. 1 sysadmin sysadmin 8 Oct 31 13:29 mytest.txt -> test.txt
Advantage: Soft links are easier to see.
Sometimes it can be difficult to know where the hard links to a file exist. If you see a regular file with a link count that is greater than one, you can use the find command with the -inum search criteria to locate the other files that have the same inode number. To find the inode number you would first use the ls -i command:

```text
sysadmin@localhost:~$ ls -i file.original

## 278772 file.original

sysadmin@localhost:~$ find / -inum 278772 2> /dev/null
```

/home/sysadmin/file.hard.1
/home/sysadmin/file.original
Soft links are much more visual, not requiring any extra commands beyond the ls command to determine the link:

```text
sysadmin@localhost:~$ ls -l mypasswd
```

lrwxrwxrwx. 1 sysadmin sysadmin 11 Oct 31 13:17 mypasswd -> /etc/passwd
Advantage: Soft links can link to any file.
Since each file system (partition) has a separate set of inodes, hard links cannot be created that attempt to cross file systems:

```text
sysadmin@localhost:~$ ln /boot/vmlinuz-2.6.32-358.6.1.el6.i686 Linux.Kernel
```

ln: creating hard link `Linux.Kernel' => `/boot/vmlinuz-2.6.32-358.6.1.el6.i686': Invalid cross-device link
In the previous example, a hard link was attempted to be created between a file in the /boot file system and the / file system; it failed because each of these file systems has a unique set of inode numbers that can't be used outside of the filesystem.
However, because a symbolic link points to another file using a pathname, you can create a soft link to a file in another filesystem:

```text
sysadmin@localhost:~$ ln -s /boot/vmlinuz-2.6.32-358.6.1.el6.i686 Linux.Kernel
sysadmin@localhost:~$ ls -l Linux.Kernel
```

lrwxrwxrwx. 1 sysadmin sysadmin 11 Oct 31 13:17 Linux.Kernel -> /boot/vmlinuz-2.6.32-358.6.1.el6.i686
Advantage: Soft links can link to a directory.
Another limitation of hard links is that they cannot be created on directories. The reason for this limitation is that the operating system itself uses hard links to define the hierarchy of the directory structure. The following example shows the error message that is displayed if you attempt to hard link to a directory:

```text
sysadmin@localhost:~$ ln /bin binary
```

ln: `/bin': hard link not allowed for directory
Linking to directories using a symbolic link is permitted:

```text
sysadmin@localhost:~$ ln -s /bin binary
sysadmin@localhost:~$ ls -l binary
```

lrwxrwxrwx. 1 sysadmin sysadmin 11 Oct 31 13:17 binary -> /bin

### 16.1 Introduction

During the installation process, most installers create a normal user and either give this user the permission to execute administrative commands with sudo or require the root user account password be configured as part of the installation process. Most Linux systems are configured to allow for one unprivileged (non-root) user to log in, as well as have the ability to effectively execute commands as the root user, either directly or indirectly.
If the computer is to be used by only one person, then having only one regular user account might be sufficient. However, if a computer needs to be shared by multiple people, then it is desirable to have a separate account for each person who uses it. There are several advantages to individuals having their own separate accounts:
Accounts can be used to grant selective access to files or services. For example, the user of each account has a separate home directory that is generally not accessible to the other users.
The sudo command can be configured to grant the ability to execute select administrative commands. If users are required to use the sudo command to perform administrative commands, then the system logs when users perform these commands.
Each account can have group memberships and rights associated with it allowing for greater management flexibility.
On some distributions, creating a new user account also automatically creates a group account for the user, called a User Private Group (UPG). On these systems, the group and username would be the same, and the only member of this new group would be the new user.
For distributions that do not create a UPG, new users are typically given the users group as their primary group. The administrator can manually create group accounts that are private for the user, but it's more common for the administrator to create groups for multiple users that need to collaborate. User accounts can be modified at any time to add or remove them from group account memberships, but users must belong to at least one group for use as their primary group.
Before you begin creating users, you should plan how to use groups. Users can be created with memberships in groups that already exist, or existing users can be modified to have memberships in existing groups.
If you already have planned which users and groups you want, it is more efficient to create your groups first and create your users with their group memberships. Otherwise, if you create your users first, and then your groups, you'll need to take an extra step to modify your users to make them members of your groups.

### 16.2 Groups

The most common reason to create a group is to provide a way for users to share files. For example, if several people who work together on the same project and need to be able to collaborate on documents stored in files for the project. In this scenario, the administrator can make these people members of a common group, change the directory ownership to the new group and set permissions on the directory that allows members of the group to access the files.
After creating or modifying a group, you can verify the changes by viewing the group configuration information in the /etc/group file with the grep command. If working with network-based authentication services, then the getent command can show you both local and network-based groups.
grep pattern filename
getent database record
For local usage, these commands show the same result, in this case for the root group:

```text
root@localhost:~# grep root /etc/group
```

root:x:0:

```text
root@localhost:~# getent group root
```

root:x:0:

### 16.3 Users

User account information is stored in the /etc/passwd file and user authentication information (password data) is stored in the /etc/shadow file. Creating a new user can be accomplished by manually adding a new line to each of these files, but that is generally not the recommended technique.
By using an appropriate command to add a new user, these files can be modified automatically and safely. If you were to modify these files manually, you would risk making a mistake that could prevent all users from being able to log in normally.
Before you begin creating users for your system, you should verify or establish practical values that are used by default with the useradd command. These settings can be found in the configuration files that are used by the useradd command.
Ensuring that the values in these configuration files are reasonable before adding users can help save you the time and trouble of having to correct user account settings after adding the users.

### 15.1 Introduction

User accounts are designed to provide security on a Linux operating system. Each person on the system must log in using a user account which either allows the person to access specific files and directories or disallows such access, accomplished using file permissions, which are file and directory permissions given by the system to users, groups and everyone else who logs in. These permissions can be edited by the root user.
User accounts also belong to groups, which can also be used to provide access to files/directories. Each user belongs to at least one group (often many) to allow users to more easily share data that is stored in files with other users.
User and group account data is stored in database files. Knowing the content of these files allows you to better understand which users have access to files and directories on the system. These database files also contain vital security information that may affect the ability of a user to log in and access the system.
Several commands provide the ability to see user and group account information, as well as to switch from one user account to another (provided you have the appropriate authority to do so). These commands are valuable for investigating usage of the system, troubleshooting system problems and for monitoring unauthorized access to the system.

### 15.2 Administrative Accounts

There are many different ways to execute a command that requires administrative or root privileges. Logging in to the system as the root user allows you to execute commands as the administrator. This access is potentially dangerous because you may forget that you are logged in as root and might run a command that could cause problems on the system. As a result, it is not recommended to log in as the root user directly.
Because using the root account is potentially dangerous, you should only execute commands as root if administrative privileges are needed. If the root account is disabled, as it is on the Ubuntu distribution, then administrative commands can be executed using the sudo command. If the root account is enabled, then a regular user can execute the su command to switch accounts to the root account.
When you log in to the system directly as root to execute commands, then everything about your session runs as the root user. If using the graphical environment, this is especially dangerous as the graphical login process is comprised of many different executables (programs that run during login). Each program that runs as the root user represents a greater threat than a process run as a standard user, as those programs would be allowed to do nearly anything, whereas standard user programs are very restricted in what they can do.
The other potential danger with logging into the system as root is that a person that does this may forget to log out to do their non-administrative work, allowing programs such as browsers and email clients to be run as the root user without restrictions on what they could do. The fact that several distributions of Linux, notably Ubuntu, do not allow users to log in as the root user should be enough indication that this is not the preferred way to perform administrative tasks.

### 15.3 User Accounts

There are several text files in the /etc directory that contain the account data of the users and groups defined on the system. For example, to see if a specific user account has been defined on the system, then the place to check is the /etc/passwd file.
The /etc/passwd file defines some of the account information for user accounts. The following example shows the last five lines of a typical /etc/passwd file:

```text
sysadmin@localhost:~$ tail -5 /etc/passwd
```

syslog:x:101:103::/home/syslog:/bin/false
bind:x:102:105::/var/cache/bind:/bin/false
sshd:x:103:65534::/var/run/sshd:/usr/sbin/nologin
operator:x:1000:37::/root:/bin/sh
sysadmin:x:1001:1001:System Administrator,,,,:/home/sysadmin:/bin/bash
Each line contains information pertaining to a single user. The data is separated into fields by colon characters. The following describes each of the fields in detail, from left to right, using the last line of the output of the previous graphic:
1. Name
sysadmin:x:1001:1001:System Administrator,,,,:/home/sysadmin:/bin/bash
The first field contains the name of the user or the username. This name is used when logging in to the system and when file ownership is viewed with the ls -l command. It is provided to make it easier for regular users to refer to the account, while the system typically utilizes the user ID internally.
2. Password Placeholder
sysadmin:x:1001:1001:System Administrator,,,,:/home/sysadmin:/bin/bash
At one time, the password for the user was stored in this location, however, now the x in this field indicates to the system that the password is in the /etc/shadow file.
3. User ID
sysadmin:x:1001:1001:System Administrator,,,,:/home/sysadmin:/bin/bash
Each account is assigned a user ID (UID). Usernames are not directly used by the system, which typically defines the account by the UID instead. For example, files are owned by UIDs, not by usernames.
4. Primary Group ID
sysadmin:x:1001:1001:System Administrator,,,,:/home/sysadmin:/bin/bash
This field indicates that the user is a member of that group, which means the user has special permissions on any file that is owned by this group.
5. Comment
sysadmin:x:1001:1001:System Administrator,,,,:/home/sysadmin:/bin/bash
This field can contain any information about the user, including their real name or other useful information.
6. Home Directory
sysadmin:x:1001:1001:System Administrator,,,,:/home/sysadmin:/bin/bash
This field defines the location of the user's home directory. For regular users, this would typically be /home/username. For example, a username of bob would have a home directory of /home/bob.
The root user usually has a different place for the home directory, the /root directory.
7. Shell
sysadmin:x:1001:1001:System Administrator,,,,:/home/sysadmin:/bin/bash
This field indicates the location of the user's login shell. By default, the user is placed in this shell whenever they log into a command line environment or open a terminal window. The bash shell /bin/bash is the most common shell for Linux users.
An efficient way to check if a specific user has been defined on a system is to search the /etc/passwd file using the grep command. For example, to see the account information for the user named sysadmin, use the following command:

```text
sysadmin@localhost:~$ grep sysadmin /etc/passwd
```

sysadmin:x:1001:1001:System Administrator,,,,:/home/sysadmin:/bin/bash

### 15.4 System Accounts

Users log into the system using regular user accounts. Typically, these accounts have UID values of greater than 500 (on some systems 1,000). The root user has special access to the system. This access is provided to the account with a UID of 0.
There are additional accounts that are not designed for users to log into. These accounts, typically from UID 1 to UID 499, are called system accounts, and they are designed to provide accounts for services that are running on the system.
System accounts have some fields in the /etc/passwd and /etc/shadow files that are different than other accounts. For example, system accounts rarely have home directories as they typically are not used to create or store files. In the /etc/passwd file, system accounts have a non-login program in the shell field:
sshd:x:103:65534::/var/run/sshd:/usr/sbin/nologin
In the /etc/shadow file, system accounts typically have an asterisk * character in place of the password field:
sshd:*:16874:0:99999:7:::
Most system accounts are necessary for the system to function correctly. You should not delete a system account unless you are certain that removing the account won't cause problems. Take time to learn what each system account does; system administrators are tasked with ensuring the security of the system, and that includes properly securing the system accounts.

### 15.5 Group Accounts

Your level of access to a system is not determined solely by your user account. Each user can be a member of one or more groups, which can also affect the level of access to the system.
Traditionally, UNIX systems limited users to belonging to no more than a total of sixteen groups, but the recent Linux kernels support users with over sixty-five thousand group memberships.
The /etc/passwd file defines the primary group membership for a user. Supplemental group membership (or secondary group membership) and the groups themselves are defined in the /etc/group file.
The /etc/group file is another colon-delimited file. The following describes the fields in more detail, using a line that describes a typical group account.
1. Group Name
mail:x:12:mail,postfix
This field contains the group name. As with usernames, names are more natural for people to remember than numbers. The system typically uses group IDs rather than group names.
2. Password Placeholder
mail:x:12:mail,postfix
While there are passwords for groups, they are rarely used in Linux. If the administrator makes a group password, it would be stored in the /etc/gshadow file. The x in this field is used to indicate that the password is not stored in this file.
3. GID
mail:x:12:mail,postfix
Each group is associated with a unique group ID (GID) which is placed in this field.
4. User List
mail:x:12:mail,postfix
This last field is used to indicate who is a member of the group. While primary group membership is defined in the /etc/passwd file, users who are assigned to additional groups would have their username placed in this field of the /etc/group file. In this case, the mail and postfix users are secondary members of the mail group.
It is very common for a username to also appear as a group name. It is also common for a user to belong to a group with the same name.
To view information about a specific group, either the grep or getent commands can be used. For example, the following commands display the mail group account information:

```text
sysadmin@localhost:~$ grep mail /etc/group
```

mail:x:12:mail,postfix

```text
sysadmin@localhost:~$ getent group mail
```

mail:x:12:mail,postfix

### 15.6 Viewing User Information

The id command is used to print user and group information for a specified user.
id [options] username
When switching between different user accounts, it can be confusing as to which account is currently logged in. When executed without an argument, the id command outputs information about the current user, allowing you to confirm your identity on the system.

```text
sysadmin@localhost:~$ id
```

uid=1001(sysadmin) gid=1001(sysadmin) groups=1001(sysadmin),4(adm),27(sudo)
The output of the id command always lists the user account information first, using the user ID and username first:
uid=1001(sysadmin) gid=1001(sysadmin) groups=1001(sysadmin),4(adm),27(sudo)
After the username the primary group is listed, denoted by both the group ID and group name:
uid=1001(sysadmin) gid=1001(sysadmin) groups=1001(sysadmin),4(adm),27(sudo)
Other information listed includes the groups the user belongs to, again denoted by group IDs followed by the group names. The user shown belongs to three groups:
uid=1001(sysadmin) gid=1001(sysadmin) groups=1001(sysadmin),4(adm),27(sudo)
If the command is given a username as an argument, such as root, it displays information about the specified account:

```text
sysadmin@localhost:~$ id root
```

uid=0(root) gid=0(root) groups=0(root)
To print only the user's primary group, use the -g option: ⁠⁠

```text
sysadmin@localhost:~$ id -g
```

1001
The id command can also be used to verify the user's secondary group memberships using the -G option. This will print all the groups that a user belongs to, both primary and secondary.

```text
sysadmin@localhost:~$ id -G

## 1001 4 27

```

The output of the previous example aligns with the contents of the /etc/group file, as a search for sysadmin reveals:

```text
sysadmin@localhost:~$ cat /etc/group | grep sysadmin
```

adm:x:4:syslog,sysadmin
sudo:x:27:sysadmin
sysadmin:x:1001:

### 15.7 Viewing Current Users

The who command displays a list of users who are currently logged into the system, where they are logged in from, and when they logged in. Through the use of options, this command is also able to display information such as the current runlevel (a functional state of the computer) and the time that the system was booted.
For example:

```text
sysadmin@localhost:~$ who
```

root            tty2        2013-10-11 10:00
sysadmin        tty1        2013-10-11 09:58 (:0)
sysadmin        pts/0       2013-10-11 09:59 (:0.0)
sysadmin        pts/1       2013-10-11 10:00 (example.com)
The following describes the output of the who command:
1. Username
root               tty2        2013-10-11 10:00
This column indicates the name of the user who is logged in. Note that by "logged in" we mean "any login process and open terminal window".
2. Terminal
root               tty2        2013-10-11 10:00
sysadmin           pts/0        2013-10-11 09:59 (:0.0)
This column indicates which terminal window the user is working in.
If the terminal name starts with tty, then this is an indication of a local login, as this is a regular command line terminal. If the terminal name starts with pts, then this indicates the user is using a pseudo terminal or running a process that acts as a terminal.
3. Date
root               tty2        2013-10-11 10:00
This column indicates when the user logged in.
4. Host
After the date and time, some location information may appear. If the location information contains a hostname, domain name or IP address, then the user has logged in remotely:
sysadmin        pts/1       2013-10-11 10:00 (example.com)
If there is a colon and a number, then this indicates that they have performed a local graphical login:
sysadmin     tty1        2013-10-11 09:59 (:0)
If no location information is shown in the last column, then this means the user logged in via a local command line process:
root               tty2        2013-10-11 10:00

> **Consider This**
>
The who command has several options for displaying system status information. For example, the -b option shows the last time the system started (booted), and the -r option shows the time the system reached the current runlevel:

```text
sysadmin@localhost:~$ who -b -r
```

system boot    2013-10-11 09:54
run-level 5    2013-10-11 09:54
There may be instances where more information about users, and what they are doing on the system, is needed. The w command provides a more detailed list about the users currently on the system than the who command. It also provides a summary of the system status. For example:

```text
sysadmin@localhost:~$ w
```

10:44:03 up 50 min,  4 users,  load average: 0.78, 0.44, 0.19

```text
USER            TTY     FROM        LOGIN@   IDLE       JCPU    PCPU    WHAT
```

root            tty2    -           10:00    43:44      0.01s   0.01s   -bash
sysadmin        tty1    :0          09:58    50:02      5.68s   0.16s   pam: gdm-password
sysadmin        pts/0   :0.0        09:59    0.00s      0.14s   0.13s   ssh 192.168.1.2
sysadmin        pts/1   example.com 10:00    0.00s      0.03s   0.01s   w
The first line of output from the w command is identical to that of the uptime command. It shows the current time, how long the system has been running, the total number of users currently logged on and the load on the system averaged over the last 1, 5 and 15 minute time periods. Load average is CPU utilization where, for a single-core system, a value of 1 would mean 100% CPU usage during that period of time. For a dual-core system, it would mean 50% CPU usage, and for a quad-core system, it would mean 25% CPU usage.
The following describes the rest of the output of the w command:
Column	Example	Description
USER	root	The name of the user who is logged in.
TTY	tty2	Which terminal window the user is working in.
FROM	example.com	Where the user logged in from.
LOGIN@	10:00	When the user logged in.
IDLE	43:44	How long the user has been idle since the last command was executed.
JCPU	0.01s	The total cpu time used by all processes run since login.
PCPU	0.01s	The total cpu time for the current process.
WHAT	-bash	The current process that the user is running.

> **Note**
>
The s character represents seconds.

### 15.8 Viewing Login History

The last command reads the entire login history from the /var/log/wtmp file and displays all logins and reboot records by default. An interesting detail of the reboot records is that it displays the version of the Linux kernel that was booted instead of the login location. The /var/log/wtmp file keeps a log of all users who have logged in and out the system.

```text
sysadmin@localhost:~$ last
```

sysadmin console Tue Sep 18 02:31   still logged in
sysadmin console                    Tue Sep 18 02:31 - 02:31  (00:00)
wtmp begins Tue Sep 18 02:31:57 2018
The last command is slightly different from the who and w commands. By default, it also shows the username, terminal, and login location, not just of the current login sessions, but previous sessions as well. Unlike the who and w commands, it displays the date and time the user logged into the system. If the user has logged off the system, then it will display the total time the user spent logged in, otherwise it will display still logged in.

> **Consider This**
>
The who command reads from the /var/log/utmp file which logs current users, while the last command reads from the /var/log/wtmp file, which keeps a history of all user logins.

### 15.8 Viewing Login History

The last command reads the entire login history from the /var/log/wtmp file and displays all logins and reboot records by default. An interesting detail of the reboot records is that it displays the version of the Linux kernel that was booted instead of the login location. The /var/log/wtmp file keeps a log of all users who have logged in and out the system.

```text
sysadmin@localhost:~$ last
```

sysadmin console Tue Sep 18 02:31   still logged in
sysadmin console                    Tue Sep 18 02:31 - 02:31  (00:00)
wtmp begins Tue Sep 18 02:31:57 2018
The last command is slightly different from the who and w commands. By default, it also shows the username, terminal, and login location, not just of the current login sessions, but previous sessions as well. Unlike the who and w commands, it displays the date and time the user logged into the system. If the user has logged off the system, then it will display the total time the user spent logged in, otherwise it will display still logged in.

> **Consider This**
>
The who command reads from the /var/log/utmp file which logs current users, while the last command reads from the /var/log/wtmp file, which keeps a history of all user logins.

### 13.2 Processes

The kernel provides access to information about active processes through a pseudo filesystem that is visible under the /proc directory. Hardware devices are made available through special files under the /dev directory, while information about those devices can be found in another pseudo filesystem under the /sys directory.
Pseudo filesystems appear to be real files on disk but exist only in memory. Most pseudo file systems such as /proc are designed to appear to be a hierarchical tree off the root of the system of directories, files and subdirectories, but in reality only exist in the system's memory, and only appear to be resident on the storage device that the root file system is on.
The /proc directory not only contains information about running processes, as its name would suggest, but it also contains information about the system hardware and the current kernel configuration.
The /proc directory is read, and its information utilized by many different commands on the system, including but not limited to top, free, mount, umount and many many others. It is rarely necessary for a user to mine the /proc directory directly—it’s easier to use the commands that utilize its information.
See an example output below:

```text
sysadmin@localhost:~$ ls /proc

## 1 cpuinfo irq modules sys

## 128 crypto kallsyms mounts sysrq-trigger

## 17 devices kcore mtrr sysvipc

## 21 diskstats key-users net thread-self

## 23 dma keys pagetypeinfo timer_list

## 39 driver kmsg partitions timer_stats

## 60 execdomains kpagecgroup sched_debug tty

## 72 fb kpagecount schedstat uptime

```

acpi       filesystems  kpageflags   scsi          version
buddyinfo  fs           loadavg      self          version_signature
bus        interrupts   locks        slabinfo      vmallocinfo
cgroups    iomem        mdstat       softirqs      vmstat
cmdline    ioports      meminfo      stat          zoneinfo
consoles   ipmi         misc         swaps
The output shows a variety of named and numbered directories. There is a numbered directory for each running process on the system, where the name of the directory matches the process ID (PID) for the running process.
For example, the numerals 72 denote PID 72, a running program, which is represented by a directory of the same name, containing many files and subdirectories that describe that running process, it’s configuration, use of memory, and many other items.
On a running Linux system, there is always a process ID or PID 1.
There are also a number of regular files in the /proc directory that provide information about the running kernel:
File	Contents

```text
/proc/cmdline	Information that was passed to the kernel when it was first started, such as command line parameters and special instructions
/proc/meminfo	Information about the use of memory by the kernel
/proc/modules	A list of modules currently loaded into the kernel to add extra functionality
```

Again, there is rarely a need to view these files directly, as other commands offer more user-friendly output and an alternative way to view this information.

> **Consider This**
>
While most of the "files" underneath the /proc directory cannot be modified, even by the root user, the "files" underneath the /proc/sys directory are potentially meant to be changed by the root user. Modifying these files changes the behavior of the Linux kernel.
Direct modification of these files causes only temporary changes to the kernel. To make changes permanent (persistent even after rebooting), entries can be added to the appropriate section of the /etc/sysctl.conf file.
For example, the /proc/sys/net/ipv4 directory contains a file named icmp_echo_ignore_all. If that file contains a zero 0 character, as it normally does, then the system will respond to icmp requests. If that file contains a one 1 character, then the system will not respond to icmp requests:

```text
sysadmin@localhost:~$ su -
Password:
root@localhost:~# cat /proc/sys/net/ipv4/icmp_echo_ignore_all
```

0

```text
root@localhost:~# ping -c1 localhost
```

PING localhost.localdomain (127.0.0.1) 56(84) bytes of data.

## 64 bytes from localhost.localdomain (127.0.0.1): icmp_seq=1 ttl=64 time=0.026 ms

```text
--- localhost.localdomain ping statistics ---

## 1 packets transmitted, 1 received, 0% packet loss, time 0ms

```

rtt min/avg/max/mdev = 0.026/0.026/0.026/0.000 ms

```text
root@localhost:~# echo 1 > /proc/sys/net/ipv4/icmp_echo_ignore_all
root@localhost:~# ping -c1 localhost
```

PING localhost.localdomain (127.0.0.1) 56(84) bytes of data.

```text
--- localhost.localdomain ping statistics ---

## 1 packets transmitted, 0 received, 100% packet loss, time 10000ms

### 13.3 Memory

```

Memory on a modern Linux system is governed and managed by the kernel. The hardware memory on the system is shared by all the processes on the system, through a method called virtual addressing. The physical memory can be referenced by a number of processes, any of which may think they are able to address more memory than they actually can. Virtual addressing allows many processes to access the same memory without conflicts or crashes. It does this by allocating certain areas of a physical (or virtual) hard disk to be used in place of physical RAM. Memory is divided into blocks of equally sized units that can be addressed like any other resource on the system. Not only can the system access memory from local system addresses, but it can also access memory that is located elsewhere, such as on a different computer, a virtual device, or even on a volume that is physically located on another continent!
While a detailed review of Linux memory addressing is beyond the scope of this course, it’s important to note the difference between user space and kernel space. Kernel space is where code for the kernel is stored and executed. This is generally in a “protected” range of memory addresses and remains isolated from other processes with lower privileges. User space, on the other hand, is available to users and programs. They communicate with the Kernel through “system call” APIs that act as intermediaries between regular programs and the Kernel. This system of separating potentially unstable or malicious programs from the critical work of the Kernel is what gives Linux systems the stability and resilience that application developers rely on.

### 13.4 Log Files

As the kernel and various processes run on the system, they produce output that describes how they are running. Some of this output is displayed as standard output and error in the terminal window where the process was executed, though some of this data is not sent to the screen. Instead, it is written to various files. This information is called log data or log messages.
Log files are useful for many reasons; they help troubleshoot problems and determine whether or not unauthorized access has been attempted.
Some processes can log their own data to these files, other processes rely on a separate process (a daemon) to handle these log data files.

> **Note**
>
Syslog is the term that is used almost generically to describe logging in Linux systems as it has been in place quite some time. In some cases, when an author says syslog what they really mean is whatever logging system is currently in use on this distribution.
Logging daemons differ in two main ways in recent distributions. The older method of doing system logging is two daemons (named syslogd and klogd) working together, but in more recent distributions, a single service named rsyslogd combines these two functions and more into a single daemon.
In yet more recent distributions, those based on systemd, the logging daemon is named journald, and the logs are designed to allow for mainly text output, but also binary. The standard method for viewing journald-based logs is to use the journalctl command.
Regardless of what the daemon process being used, the log files themselves are almost always placed into the /var/log directory structure. Although some of the file names may vary, here are some of the more common files to be found in this directory:
File	Contents
boot.log	Messages generated as services are started during the startup of the system.
cron	Messages generated by the crond daemon for jobs to be executed on a recurring basis.
dmesg	Messages generated by the kernel during system boot up.
maillog	Messages produced by the mail daemon for e-mail messages sent or received.
messages	Messages from the kernel and other processes that don't belong elsewhere. Sometimes named syslog instead of messages after the daemon that writes this file.
secure	Messages from processes that required authorization or authentication (such as the login process).
journal	Messages from the default configuration of the systemd-journald.service; can be configured in the /etc/journald.conf file amongst other places.
Xorg.0.log	Messages from the X Windows (GUI) server.
You can view the contents of various log files using two different methods. First, as with most other files, you can use the cat command, or the less command to allow for searching, scrolling and other options.
The second method is to use the journalctl command on systemd-based systems, mainly because the /var/log/journal file now often contains binary information and using the cat or less commands may produce confusing screen behavior from control codes and binary items in the log files.
Log files are rotated, meaning older log files are renamed and replaced with newer log files. The file names that appear in the table above may have a numeric or date suffix added to them: for example, secure.0 or secure-20181103.
Rotating a log file typically occurs on a regularly-scheduled basis: for example, once a week. When a log file is rotated, the system stops writing to the log file and adds a suffix to it. Then a new file with the original name is created, and the logging process continues using this new file.
With most modern daemons, a date suffix is used. So, at the end of the week ending November 3, 2018, the logging daemon might stop writing to /var/log/messages (or /var/log/journal), rename that file /var/log/messages-20181103, and then begin writing to a new /var/log/messages file.
Although most log files contain text as their contents, which can be viewed safely with many tools, other files such as the /var/log/btmp and /var/log/wtmp files contain binary. By using the file command, users can check the file content type before they view it to make sure that it is safe to view. The following file command classifies /var/log/wtmp as data, which usually means the file is binary:

```text
sysadmin@localhost:~$ file /var/log/wtmp
```

/var/log/wtmp: data
For the files that contain binary data, there are commands available that will read the files, interpret their contents and then output text. For example, the lastb and last commands can be used to view the /var/log/btmp and /var/log/wtmp files respectively.
The lastb requires root privileges to be executed in our virtual machine environment.

### 13.5 Kernel Messages

The /var/log/dmesg file contains the kernel messages that were produced during system startup. The /var/log/messages file contains kernel messages that are produced as the system is running, but those messages are mixed in with other messages from daemons or processes.
Although the kernel doesn't have its own log file normally, one can be configured for it by modifying either the /etc/syslog.conf file or the /etc/rsyslog.conf file. In addition, the dmesg command can be used to view the kernel ring buffer, which holds a large number of messages that are generated by the kernel.‌⁠​​⁠​
On an active system, or one experiencing many kernel errors, the capacity of this buffer may be exceeded, and some messages might be lost. The size of this buffer is set at the time the kernel is compiled, so it is not trivial to change.
Executing the dmesg command can produce up to 512 kilobytes of text, so filtering the command with a pipe to another command like less or grep is recommended. For example, if a user were troubleshooting problems with a USB device, then searching for the text USB with the grep command is helpful. The -i option is used to ignore case:

```text
sysadmin@localhost:~$ dmesg | grep -i usb
```

usbcore: registered new interface driver usbfs
usbcore: registered new interface driver hub
usbcore: registered new device driver usb
ehci_hcd: USB 2.0 'Enhanced' Host Controller (EHCI) Driver
ohci_hcd: USB 1.1 'Open' Host Controller (OHCI) Driver
ohci_hcd 0000:00:06.0: new USB bus registered, assigned bus number 1
usb usb1: New USB device found, idVendor=1d6b, idProduct=0001
usb usb1: New USB device strings: Mfr=3, Product=2, SerialNumber=1

### 13.6 Filesystem Hierarchy Standard

Among the standards supported by the Linux Foundation is the Filesystem Hierarchy Standard (FHS), which is hosted at the URL http://www.pathname.com/fhs/.
A standard is a set of rules or guidelines that it is recommended to follow. However, these guidelines certainly can be broken, either by entire distributions or by administrators on individual machines.
The FHS standard categorizes each system directory in a couple of ways:
- A directory can be categorized as either shareable or not, referring to whether the directory can be shared on a network and used by multiple machines.
- The directory is put into a category of having either static files (file contents won't change) or variable files (file contents can change).
To make these classifications, it is often necessary to refer to subdirectories below the top level of directories. For example, the /var directory itself cannot be categorized as either shareable or not shareable, but one of its subdirectories, the /var/mail directory, is shareable. Conversely, the /var/lock directory should not be shareable.
Not Shareable	Shareable
Variable	/var/lock	/var/mail
Static	/etc	/opt

The FHS standard defines four hierarchies of directories used in organizing the files of the filesystem. The top-level or root hierarchy follows:
Directory	Contents

```text
/	The base of the structure, or root of the filesystem, this directory unifies all directories regardless of whether they are local partitions, removable devices or network shares
/bin	Essential binaries like the ls, cp, and rm commands, and be a part of the root filesystem
/boot	Files necessary to boot the system, such as the Linux kernel and associated configuration files
/dev	Files that represent hardware devices and other special files, such as the /dev/null and /dev/zero files
/etc	Essential host configurations files such as the /etc/hosts or /etc/passwd files
/home	User home directories
/lib	Essential libraries to support the executable files in the /bin and /sbin directories
/lib64	Essential libraries built for a specific architecture. For example, the /lib64 directory for 64-bit AMD/Intel x86 compatible processors
/media	Mount point for removable media mounted automatically
/mnt	Mount point for temporarily mounting filesystems manually
/opt	Optional third-party software installation location
/proc	Virtual filesystem for the kernel to report process information, as well as other information
/root	Home directory of the root user
/sbin	Essential system binaries primarily used by the root user
/sys	Virtual filesystem for information about hardware devices connected to the system
/srv	Location where site-specific services may be hosted
/tmp	Directory where all users are allowed to create temporary files and that is supposed to be cleared at boot time (but often is not)
/usr	Second hierarchy
```

Non-essential files for multi-user use

```text
/usr/local	Third hierarchy
```

Files for software not originating from distribution

```text
/var	Fourth hierarchy
```

Files that change over time

```text
/var/cache	Files used for caching application data
/var/log	Most log files
/var/lock	Lock files for shared resources
/var/spool	Spool files for printing and mail
/var/tmp	Temporary files to be preserved between reboots
```

The second and third hierarchies, located under the /usr and /usr/local directories, repeat the pattern of many of the key directories found under the first hierarchy or root filesystem. The fourth hierarchy, the /var directory, also repeats some of the top-level directories such as lib, opt and tmp.
While the root filesystem and its contents are considered essential or necessary to boot the system, the /var, /usr and /usr/local directories are deemed non-essential for the boot process. As a result, the root filesystem and its directories may be the only ones available in certain situations like booting into single-user mode, an environment designed for troubleshooting the system.
The /usr directory is intended to hold software for use by multiple users. The /usr directory is sometimes shared over the network and mounted as read-only.
The /usr/local hierarchy is for installation of software that does not originate with the distribution. Often this directory is used for software that is compiled from the source code.

#### 13.6.1 Organization Within the Filesystem Hierarchy

Although the FHS standard is helpful for a detailed understanding of the layout of the directories used by most Linux distributions, the following provides a more generalized description of the layout of directories as they exist on a typical Linux distribution.
User Home Directories
The /home directory has a directory underneath it for each user account. For example, a user bob will have a home directory of /home/bob. Typically, only the user bob will have access to this directory. Without being assigned special permissions on other directories, a user can only create files in their home directory, the /tmp directory, and the /var/tmp directory.
Binary Directories
Binary directories contain the programs that users and administrators execute to start processes or applications running on the system.
User-Specific Binaries
The binary directories that are intended to be used by non-privileged users include:
- /bin
- /usr/bin
- /usr/local/bin
Sometimes third-party software also store their executable files in directories such as:
- /usr/local/application/bin
- /opt/application/bin
In addition, it is not unusual for each user to have their own bin directory located in their home directory; for example, /home/bob/bin.
Root-Restricted Binaries
On the other hand, the sbin directories are primarily intended to be used by the system administrator (the root user). These usually include:
- /sbin
- /usr/sbin
- /usr/local/sbin
Some third-party administrative applications could also use directories such as:
- /usr/local/application/sbin
- /opt/application/sbin
Depending on the distribution, the PATH variable may not contain all of the possible bin and sbin directories. To execute a command in one of these directories, the directory needs to be included in the PATH variable list, or the user needs to specify the path to the command.
Software Application Directories
Unlike the Windows operating system, where applications may have all of their files installed in a single subdirectory under the C:\Program Files directory, applications in Linux may have their files in multiple directories spread out throughout the Linux filesystem. For Debian-derived distributions, you can execute the dpkg -L packagename command to get the list of file locations. In Red Hat-derived distributions, you can run the rpm -ql packagename command for the list of the locations of the files that belong to that application.
The executable program binary files may go in the /usr/bin directory if they are included with the operating system, or else they may go into the /usr/local/bin or /opt/application/bin directories if they came from a third party.
The data for the application may be stored in one of the following subdirectories:
- /usr/share
- /usr/lib
- /opt/application
- /var/lib
The file related to documentation may be stored in one of the following subdirectories:
- /usr/share/doc
- /usr/share/man
- /usr/share/info
The global configuration files for an application are most likely to be stored in a subdirectory under the /etc directory, while the personalized configuration files (specific for a user) for the application are probably in a hidden subdirectory of the user's home directory.
Library Directories
Libraries are files which contain code that is shared between multiple programs. Most library file names end in a file extension of .so, which means shared object.
Multiple versions of a library may be present because the code may be different within each file even though it may perform similar functions as other versions of the library. One of the reasons that the code may be different, even though it may do the same thing as another library file, is that it is compiled to run on a different kind of processor. For example, it is typical for systems that use code designed for 64-bit Intel/AMD type processors to have both 32-bit libraries and 64-bit libraries.
The libraries that support the essential binary programs found in the /bin and /sbin directories are typically located in either /lib or /lib64.
To support the /usr/bin and /usr/sbin executables, the /usr/lib and /usr/lib64 library directories are typically used.
For supporting applications that are not distributed with the operating system, the /usr/local/lib and /opt/application/lib library directories are frequently used.
Variable Data Directories
The /var directory and many of its subdirectories can contain data that changes frequently. If your system is used for email, then either /var/mail or /var/spool/mail is normally used to store users' email data. If you are printing from your system, then the /var/spool/cups directory is used to store the print jobs temporarily.
Depending on what events are being logged and how much activity is occurring, the system determines how large your log file becomes. On a busy system, there could be a considerable amount of data in the log files. These files are stored in the /var/log directory.
While the log files can be handy for troubleshooting problems, they can cause problems. One major concern for all of these directories is that they can fill up the disk space quickly on an active system. If the /var directory is not a separate partition, then the root filesystem could become full and cause the system to crash.
