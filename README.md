# Getting Started with VirtualBox

## Story

Your boss has sent you what she called a _virtual machine image_ and told you to take a look whether it works or should she throw it in the dust bin, because she doesn't have any time for this "non-sense".

Little did she know this will spark a never ceasing interest in you towards learning about virtualization, Linux, networking, DevOps ... _and the list goes on!_

## What are you going to learn?

- How to install a hypervisor (VirtualBox) on your host machine
- What does "host" and "guest" mean
- What are virtual machine images
- What's the benefit of using pre-made images
- Import and start new virtual machine/appliance from ready-made image
- Understand what is a VM snapshot
- How to take/restore snapshots of virtual machines
- Learn about the existence VirtualBox manual

## Tasks

1. Install Oracle's open-source type-2 hypervisor called "VirtualBox" on your computer. [Download the installer and the extension from here.](https://www.virtualbox.org/wiki/Downloads)
    - The latest version (6 or later) of VirtualBox is installed on the host machine
    - The latest version (matching VirtualBox's version) of the Oracle Extension Pack is installed into VirtualBox

2. Obtain a ready-made virtual machine image to get started with virtualization.
    - This [virtual machine image](https://github.com/CodecoolBase/short-admin-vms/releases/latest/download/ubuntu-18.04-base.ova) is downloaded onto the host machine

3. Use the virtual machine image to create a virtual machine/appliance.
    - The previously downloaded image is imported into VirtualBox as a new virtual machine/appliance
    - A snapshot called "Snapshot 1" is created of the virtual machine while it is in a stopped state

4. Start the virtual machine and verify that it works expected.
    - The virtual machine is started and OS booted
    - Using `ubuntu` as username and `ubuntu` as password a login session has been started
    - A screenshot is made with VirtualBox and saved on the host machine while in the guest the current time is visible by entering `date` command

## General requirements

None

## Hints

- The virtual machines you start and interact with via the VirtualBox GUI (based on the `.ova` files we're providing you with) **by default use an English keyboard layout**, to change this **execute `sudo chlang hu`** or some other language suitable for you in the _virtual terminal_ (*note*: that when _SSH-ing_ into the machine this won't be an issue)
- When downloading VirtualBox choose the appropriate build/installer, most probably this will be the 64-bit/x64 version
- During its installation process, VirtualBox is going to install virtual network adapters on to your host machine, this is normal and should be allowed
- When importing the virtual image you may receive errors regarding the virtual network adapter used telling you it _Could not start the machine_ because some _network interfaces were not found_. In case this happens click on _Change Network Settings_ in the error popup window and simply save the settings (your default network card will be selected automatically)
- There are a few ways to start a virtual machine (normal, headless, detachable). Choose normal for this project
- **When you are reading background materials:**
  - [What is a Virtual Machine?](https://www.reddit.com/r/explainlikeimfive/comments/1a86vh/eli5_what_is_a_virtual_machine_how_does_it_work/) - Only the first few answers are important
  - [Virtual appliance](https://en.wikipedia.org/wiki/Virtual_appliance) - The first paragraph of the page is the most important

## Background materials

- <i class="far fa-exclamation"></i> [How to Use VirtualBox (Beginners Guide)](https://www.youtube.com/watch?v=sB_5fqiysi4)
- [What is a Virtual Machine?](https://www.reddit.com/r/explainlikeimfive/comments/1a86vh/eli5_what_is_a_virtual_machine_how_does_it_work/)
- <i class="far fa-exclamation"></i> [Virtual appliance](https://en.wikipedia.org/wiki/Virtual_appliance)
- <i class="far fa-exclamation"></i> [Host vs. Guest OS](https://www.datto.com/library/whats-the-difference-host-vs-guest-os)
- <i class="far fa-exclamation"></i> [Create and restore from a snapshot in VirtualBox 6](https://www.youtube.com/watch?v=KoDCXwF5cYM)
- <i class="far fa-exclamation"></i> [Virtual Machines: Pros & Cons](https://www.cynexlink.com/2017/08/18/virtual-machines-pros-cons/)
- [VirtualBox manual](https://www.virtualbox.org/wiki/Downloads#manual)
