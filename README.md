# Windows to Linux

Are you a regular person - not a techie - who uses Microsoft Windows and wants to run Linux? 

There are a lot of questions on social media from people like you. They don't want to see a lot of technobabble or debates between experienced Linux users. They don't want an open-ended answer along the lines of "you can do anything you want with Linux, so chart your own course." 

If that's you, then I hope this will help a little. It isn't meant to be a detailed tutorial. It's only meant to cut through some of the details so you can see a roadmap to get to where you want to go.

## Preliminaries 

Here are some things to consider before jumping in.

### Crucial first step

The first step is to come to grips with the fact this isn't going to be as simple as clicking on a button. Set your expectations accordingly, or you will become frustrated. If you need to take a couple of deep breaths, this is a good time.

### Helpful second step

If you have a friend or colleague who is a little more computer-savvy than you, ask them to help you do this - in person, not in the form of email or chat. If you are not technical, many issues that come up along the way will feel daunting. Having someone by your side who has some idea of what to do can save you time and frustration.

To your technical friend the issues will not seem overwhelming, but to you the experience may feel like an endless series of cryptic and scary messages and error codes. If you try to tackle it on your own, you'll need a lot of patience.

### How will you use Linux and Windows?

There are several ways to get a Linux system up and running. To choose the appropriate one, think about how you intend to use Linux and Windows. You don't have to perform an in-depth technical assessment. Just think about which of the following statements sounds like you:

- I want to replace my Windows computer with Linux. I will not use Windows anymore.
- I want to use Windows and Linux on the same computer, but I don't have to use both at the same time.
- I want to use both Windows and Linux on the same computer together.

## Replace Windows with Linux

There are two options:

- Buy a computer with Linux already installed. Here's a [list of computers with Linux preinstalled](https://linuxpreloaded.com).
- Download Linux and install it on your computer. This will replace your existing Windows system altogether. 

In both these cases, you may want to copy your files from the Windows system to the new Linux system. This is common to several of the options described here, so we'll cover it later. 

## Windows and Linux on the same computer but not at the same time 

This is called a "dual-boot" setup. When you start the computer, you tell it whether you want to run Windows or Linux. You can't use both at the same time. 

To set up a dual boot system you have to do some "technical" tasks; notably, partitioning the hard drive. It's a good idea to have someone help you with this.

Since this is relatively involved compared with the other options, and the result is actually a bit less useful than the other options, I'm not going to cover it. You can find plenty of advice online if you want to tackle this; but I'm assuming you're not technical at all, so it may be more work than you want to do.

## Windows and Linux on the same computer at the same time 

There are a couple of ways to do this. Think about whether you want a complete Linux system alongside your complete Windows system, or you just need to run a few particular Linux programs and you will otherwise use Windows for most things. 

### Run some Linux programs but mainly use Windows 

Use the Windows Subsystem for Linux (WSL) to install Linux on your Windows system. You can then install the specific Linux program(s) you need to use. Using them will feel very much like using any other program on your Windows system.

- [How to install Linux on Windows with WSL](https://learn.microsoft.com/en-us/windows/wsl/install)

The basic WSL install results in a Linux system that doesn't have any windows. I assume if you're accustomed to Microsoft Windows, you will want to use the Linux system in the same way. You can install additional software on the Linux system to support this. (GUI stands for Graphical User Interface; the thing that displays windows on the screen.)

- [Run Linux GUI apps on the Windows Subsystem for Linux](https://learn.microsoft.com/en-us/windows/wsl/tutorials/gui-apps)

This version of Linux will not have any of the general-user or consumer applications installed. You'll have to install each program you want to use. (That's not as hard as it sounds.)

### Run Linux under virtualization on Windows 

Use a virtualization program to host a complete Linux system on Windows without affecting the rest of your Windows system. 

- VirtualBox, supported by Oracle, is free for personal and educational use. It is extremely finicky and may not work well for you. [VirtualBox download page](https://www.virtualbox.org/wiki/Downloads)
- VMware Workstation, supported by Broadcom, is free for personal use. This product works much more smoothly than VirtualBox. [VMware Workstation download page](https://support.broadcom.com/group/ecx/productdownloads?subfamily=VMware+Workstation+Pro) 

Using one of these virtualization programs you can share your files between Windows and Linux. 

To use one of these products, or another product that performs a similar function, you must download an ISO file containing a Linux distribution. ISO is a file format based on the ISO 9660 standard. 

You don't have to know the internal details of that. Just know that when you are downloading an operating system, the software has to be in this format so that it can be installed on a computer. 

Many online guides for doing this advise you to "burn" (that is, _copy_) the iso to a removable device such as a thumb drive. This is so that you can install it on a physical computer. If you are using virtualization software, you don't need to do that. The virtualization software can read the iso from your hard drive.

As this step is common to several of the options described here, we'll cover it later. 

## Linux distributions, or distros 

A "distro" or _distribution_ is a particular "build" of the Linux operating system. Each distro consists of the core functionality of Linux, which is common to all of them, plus a selection of additional software to make the system usable for practical tasks. Each distro includes a different selection of additional software and sets some of the system configuration options differently by default. 

When you have asked about this on social media and been inundated with geeks arguing with each other about their favorite Linux distros instead of helping you, this is what they're talking about. In general, these debates are on the level of "What's your favorite flavor of ice cream?"

The distro that seems to be easiest for a Windows user who is a regular person is called Ubuntu Desktop. It works on desktop and laptop computers, it has windows like Microsoft Windows has, and works with a mouse and keyboard. It will not look identical to Microsoft Windows, however.

Ubuntu Desktop comes with software that performs the same general kinds of tasks as the software that comes with a Windows system. These are things like a Web browser, an office suite, a media player, and so forth. They won't be exactly the same programs as you're used to seeing on Windows, but they perform the same general functions. 

Here's the [download page for Ubuntu Desktop](https://ubuntu.com/download/desktop/thank-you?version=24.04.2&architecture=amd64&lts=true). 

The thing you'll download is an iso file. You can feed that file into your virtualization software to create a virtual Linux system, or "burn" it onto a thumb drive you can use to install it on a physical computer. 

If you're using the Windows Subsystem for Linux (WSL), you install Ubuntu through WSL instead of by downloading an iso. Check the links above under _Run some Linux programs but mainly use Windows_ for instructions.

## Transferring your data (files) 

Whenever you migrate your work from one computer to another, you need to transfer your files. 

### One Drive

If you use Windows in the standard way (according to Microsoft), then you almost certainly have One Drive, and your local files are synchronized with One Drive. There is a One Drive client for Linux, [which you can find here](https://github.com/abraunegg/onedrive). 

After installing your new Linux system, install the One Drive client on it. Then you will be able to access your files on One Drive. 

### Backup and restore

If you don't use One Drive, then make a backup of your files either using a cloud-based service or onto a physical external hard drive. Of course, if you plan to wipe out your Windows system, then make the backup first.

When migrating from one operating system (like Windows) to a different one (like Linux), it's likely that both systems can't read the same file formats. 

Windows uses a filesystem called NTFS. Your Windows files are in this format. To read them under Ubuntu, you need to install a "driver" (a kind of program that interacts with devices, such as hard drives) that understands the NTFS format. 

For Ubuntu, there's [a package called ntfs-3g](https://launchpad.net/ubuntu/+source/ntfs-3g) that does this well. Ubuntu doesn't come with this package, so you have to install it. 

## Creating a bootable USB stick (thumb drive) 

When a computer starts up, it looks on various media to find a file it recognizes as a "bootstrap" sort of file, and uses that file to initialize itself. Usually, if you insert a thumb drive before starting the machine, it will look at the thumb drive before it looks at other media. If not, then you can interrupt the "boot sequence" and tell it to look there first. (Your technical friend can help you with the details, which differ by computer.)

The iso file you downloaded is the kind of thing the computer is looking for. To get it into the right format, you have to use a special program to "burn" the iso file onto the thumb drive. It isn't a standard file, so just copying it won't do the trick. 

This Ubuntu installation tutorial [includes instructions to create a bootable USB stick](https://ubuntu.com/tutorials/install-ubuntu-desktop#1-overview).

## Installing packages on Ubuntu

A _package_ is a set of files the system uses to install a program. There are several ways to install packages on Ubuntu Linux, and [they are described here](https://www.wikihow.com/Install-Ubuntu-Packages). 

It doesn't matter which method you use. They all result in the same outcome. You can pick whichever method seems easiest for you. 






