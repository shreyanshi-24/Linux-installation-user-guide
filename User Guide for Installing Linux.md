<!-- This is the title of the doc -->
# User Guide for Installing Linux

<!-- The doc starts from here -->
## Document overview

### Purpose

The purpose of this guide is to help users successfully install Linux operating system on their computer. It provides clear, step-by-step instructions to ensure a smooth installation process and a functional system.

### What this guide covers

This guide covers:

- An introduction to operating systems and Linux.
- System requirements and preparation before installation.
- Step-by-step instructions for installing Linux.
- Post-installation setup, including basic configuration, software installation, and troubleshooting tips.

### Intended users

This guide is intended for:

- Beginners with some or no experience with Linux.
- Users who want to install Linux for personal use, learning, or development purposes.
- Anyone looking for a clear, practical, and easy-to-follow Linux installation guide.

### Additional information

- The guide assumes basic knowledge of using a computer but does not require prior Linux experience.
- Users are encouraged to back up important data before starting the installation.
- While this guide focuses on one Linux distribution, the concepts and steps are applicable to most popular Linux versions.

## Introduction to operating system

An operating system (OS) is the main software that runs on a computer. It acts as a bridge between hardware and software, enabling the computer to function. Without an OS, your computer cannot operate. The OS ensures that all parts of the system work together, which is why it is often called *the brain of the computer*.

### Why an operating system is important

An OS is important because it:

* Allows you to interact with the computer through a desktop, icons, or command line.
* Manages resources such as files, memory (RAM), and the processor (CPU).
* Runs applications such as browsers, media players, and office tools.
* Protects the system by managing passwords and permissions.

### Types of operating systems

Popular operating systems include:

1. **Windows** – Widely used on personal computers.
2. **macOS** – The operating system for Apple computers.
3. **Linux distributions (distros)** – Open-source operating systems based on the Linux kernel.
4. **Android and iOS** – Operating systems designed for mobile devices.

This guide focuses on Linux and provides instructions to install it on your system.

## Introduction to Linux

Linux is a family of operating systems based on the Linux kernel, similar to Windows or macOS. It is used on desktops, servers, smartphones, and embedded systems because of its stability, security, and flexibility.

### Key Features of Linux

- **Open source** – The source code is freely available to use, modify, and share.
- **Stable and secure** – Known for reliability and less vulnerable to viruses.
- **Flexible and customizable** – Runs on many types of devices and allows users to adapt the system to their needs.
- **Community support** – A global community provides regular updates, tools, and assistance.

### Popular Linux Distributions

Linux comes in different versions known as distributions (distros). Each distro has unique features, software management tools, and target audiences. Some popular Linux distributions include:

| Distribution | Target Users       | Key Features                                        | Ideal Use Case                  |
|--------------|-----------------|----------------------------------------------------|--------------------------------|
| **Ubuntu**   | Beginners & Desktop users | User-friendly, large community, frequent updates | Desktop, general-purpose       |
| **Fedora**   | Developers & Enthusiasts | Cutting-edge technologies, secure, stable        | Development, testing           |
| **Debian**   | Advanced & Server users   | Highly stable, large software repository         | Servers, long-term support     |
| **CentOS / Rocky Linux / AlmaLinux** | Enterprise users | Enterprise-grade, stable, secure                | Servers, production environments |
| **Arch Linux** | Advanced users          | Lightweight, highly customizable, rolling release | Learning Linux, customization  |

### Why Choose Linux?
Linux is an excellent choice if you want a **secure, flexible, and customizable operating system**. It is ideal for learning, development, hosting servers, or simply exploring a free alternative to proprietary systems.

For this guide, we recommend starting with **Ubuntu**, as it is easy to install, well-documented, and supported by a large community. This makes it ideal for new users.

## System preparation for installation

Before installing Linux, prepare your computer to ensure the installation goes smoothly and you do not lose important data.

### Check hardware requirements

Ensure your computer meets the minimum hardware requirements for Linux to run smoothly and avoid errors during installation.

#### Minimum hardware requirements for Ubuntu

| Component | Minimum | Recommended |
|-----------|---------|------------|
| CPU       | 2 GHz dual-core | 2 GHz quad-core or higher |
| RAM       | 4 GB           | 8 GB or more |
| Storage   | 25 GB          | 50 GB or more |
| Display   | Any basic GPU  | Optional: Dedicated GPU for graphics-intensive tasks |

#### How to check your hardware

| Operating System | Steps | What to Look For |
|-----------------|-------|-----------------|
| **Windows** | 1. Press `Win + R` to open the Run dialog.<br>2. Type `dxdiag` and press Enter.<br>3. Review the DirectX Diagnostic Tool information. | - **Processor:** CPU type and speed<br>- **Memory:** Installed RAM<br>- **Display:** Graphics card info (optional) |
| **macOS** | 1. Click the **Apple menu** in the top-left corner.<br>2. Select **About This Mac**.<br>3. Review the overview information. | - **Processor:** CPU type and speed<br>- **Memory (RAM):** Installed RAM<br>- **Storage:** Available disk space |

### Back up your data

Back up all important files to avoid data loss. Options include:

| Backup Method | Steps | Notes / Tips |
|---------------|-------|-------------|
| **External USB drive / hard drive** | 1. Connect the drive.<br>2. Open File Explorer (Windows) or Finder (macOS).<br>3. Copy important folders (Documents, Desktop, Pictures) to the drive.<br>4. Safely eject the drive. | Ensure sufficient storage and keep the drive safe. |
| **Cloud storage** | 1. Sign in to a cloud service (Google Drive, Dropbox, OneDrive).<br>2. Upload important files.<br>3. Verify the upload completed. | Provides off-site backup and access from any device. |
| **Disk image / system backup (advanced)** | 1. Use Macrium Reflect (Windows) or Time Machine (macOS) to create a full system backup.<br>2. Store the backup on an external drive. | Restores the entire system if needed; recommended for critical systems or advanced users. |

> **Note:** Maintain at least two backups: one local and another in the cloud.

### Choose a Linux distribution

Select the distribution (distro) that fits your needs. A distro includes the Linux kernel along with system tools, libraries, and applications.

**Considerations for choosing a distribution:**

1. **Purpose:** Desktop, server, or development.
2. **Hardware compatibility:** Some distros are lighter and better for older hardware.
3. **Community support:** A strong community helps troubleshoot issues.
4. **Software requirements:** Ensure required applications are supported.
5. **Learning curve:** Beginner-friendly distros (Ubuntu) vs. advanced distros (Arch).

Once you select a distribution, download its ISO file from the official website.

### Download the Linux ISO file

The ISO file is a complete image of the operating system used for installation.

**Steps to download the ISO:**

1. Go to the official website of your chosen Linux distribution (such as, [Ubuntu Downloads](https://ubuntu.com/download)).
2. Choose the version or edition to install. Desktop versions are recommended for personal computers; server versions are for servers.
3. Select the download method:
   - **Direct download:** Save the ISO file directly to your computer.
   - **Torrent download:** Use a torrent client for faster and more reliable download.
4. Verify the ISO file using the provided checksum (SHA256 or MD5) to ensure integrity.
5. Save the ISO file in an accessible location for installation.

> **Note:** ISO files are large (1–5 GB). Use a stable internet connection.

### Create a bootable USB drive

A bootable USB drive allows your computer to start the installation process.

**Prerequisites:**

- USB flash drive (minimum 8 GB recommended).
- Downloaded ISO file.
- USB creation tool:
  - **Windows:** Rufus ([https://rufus.ie](https://rufus.ie))
  - **Windows/Linux/macOS:** balenaEtcher ([https://www.balena.io/etcher/](https://www.balena.io/etcher/))

#### Using Rufus (Windows)

1. Insert your USB drive.
2. Open **Rufus**.
3. Under **Device**, select your USB drive.
4. Click **Select** and choose the downloaded ISO file.
5. Choose the **Partition scheme**:
   - **GPT** for UEFI systems
   - **MBR** for older BIOS systems
6. Keep the **File system** as **FAT32**.
7. Click **Start**.
8. Confirm any warnings about data loss.
9. Wait for the process to complete. The USB drive is now bootable.

#### Using balenaEtcher (Windows/Linux/macOS)

1. Insert your USB drive.
2. Open **balenaEtcher**.
3. Click **Flash from file** and select the ISO file.
4. Select the USB drive as the target.
5. Click **Flash!** and wait for completion.


## Booting from installation media

After preparing your bootable USB drive, follow these steps to start the installation:

1. **Insert the USB drive** into your computer.
2. **Restart the computer.**
3. **Access the boot menu** by pressing the appropriate key during startup. Common keys include:
   - `F12`
   - `Esc`
   - `F10`
   - `Del`
   *(Check your computer’s manual if you are unsure.)*

4. **Select your USB drive** from the list of bootable devices and press `Enter`.
5. **Wait for the installation environment** to load. You may see a prompt like "Press any key to boot from USB"; press any key if required.

## Starting the Linux installer

After booting your computer from the USB drive, follow these steps to start the Linux installer:

1. When the **Linux boot menu** appears, you may see options such as:
   - Try Linux without installing
   - Install Linux
   - Check the installation media
   - Boot from first hard disk

2. Select **Install Linux** (or the equivalent option for your distribution) and press `Enter`.

3. The installer will start and guide you through the installation process, including:
   - Selecting your language and region
   - Configuring the keyboard layout
   - Connecting to a network (optional)
   - Partitioning the disk
   - Setting up user accounts and passwords

> **Note:** Follow the on-screen instructions carefully to complete the installation process.

## Choosing installation preferences

During Linux installation, you need to select various preferences to customize your system. Follow these steps carefully.

### Select language and region

1. Choose the **language** for the installer and system.
2. Select your **region or time zone** to set the system clock and regional settings.

### Select keyboard layout

1. Choose your **keyboard layout** (for example, US, UK, or another language).
2. Optionally, test the keyboard in the provided text box to ensure it works correctly.

### Configure network

1. Connect to a **Wi-Fi or wired network** if prompted.
2. You can skip this step and configure the network after installation.

### Choose installation type / disk partitioning

**Prerequisites:** Back up important data before modifying partitions.

1. Choose how Linux will be installed on your hard drive:
   - **Erase disk and install Linux:** Automatically formats the drive and installs Linux.
   - **Install alongside existing operating system:** Sets up a dual-boot with another OS.
   - **Something else / Manual partitioning:** Advanced users can create custom partitions, such as `/`, `/home`, and `swap`.

### Set up user account

1. Enter your **name** and **username**.
2. Set a **strong password**.
3. Choose to **log in automatically** or require a password at login.

### Configure additional preferences

1. Select whether to **encrypt your home folder**.
2. Choose to **install third-party software** for media codecs and other utilities.
3. Review all selections carefully before proceeding.

### Begin installation

1. Click **Continue** or **Install Now** to start the installation.
2. The installer will copy files and configure your system according to your selected preferences.

## Disk partitioning

During Linux installation, you need to decide how the installer will use your hard drive. Disk partitioning determines how storage is divided for the operating system, files, and swap space.

You may see several options, depending on your Linux distribution:

- **Erase disk and install Linux**
  - Automatically deletes all existing data and partitions on the selected drive.
  - Recommended for new installations or computers dedicated to Linux.

- **Install alongside existing operating system**
  - Allows you to dual-boot Linux with another operating system, such as Windows.
  - The installer automatically resizes existing partitions to make space for Linux.

- **Something else / Manual partitioning**
  - Lets you manually create, delete, and configure partitions.
  - Recommended for advanced users who want custom partition layouts.

### Apply changes

1. Review your partition layout carefully.
2. Click **Install Now** or **Apply** to let the installer format and set up partitions.
3. Confirm any warnings about data loss.

## Configuring user and system settings

During installation, you will configure user details and basic system settings. These choices determine how you log in and how your system identifies itself.

### Enter user information

- **Your name:** Enter the full name of the primary user.
- **Computer name:** Set a hostname to identify your computer on a network (such as, `john-pc`).
- **Username:** Choose a short name used to log in (such as, `john`).
- **Password:** Choose a strong password. You will use this for login and administrative tasks.

### Choose login options

- **Require my password to log in:** Recommended for security.
- **Log in automatically:** Logs in without asking for a password (not recommended on shared computers).

### Set time zone and clock

- Select your **region and city** on the world map or from the drop-down list.
- The system clock is set automatically if connected to the internet.
- If offline, enter the time and date manually.

### Select keyboard layout

- Choose the appropriate **keyboard layout** (for example, US, UK, or another language).
- Test typing in the text box to confirm it matches your physical keyboard.
- Add additional layouts if needed.

### Review settings

- The installer displays a summary of your chosen settings (user, time zone, keyboard).
- Review carefully before proceeding.
- Click **Continue** or **Install Now** to start the installation.

## Completing installation

After selecting your installation preferences (language, keyboard layout, partitions, and user setup), the installer copies files and configures the system. Follow these steps to complete the process.

### Review installation summary

- The installer displays a **summary of your choices**.
- Double-check disk partitions, time zone, and user information.
- If everything is correct, click **Install Now** or **Continue**.

### Copy system files

- The installer copies system files to your hard drive.
- This may take several minutes, depending on your computer and USB/DVD speed.
- During this process, you may see a slideshow introducing Linux features.

### Install system components

After copying files, the installer performs these tasks:

- Configures the bootloader (GRUB).
- Sets up partitions and file systems.
- Installs essential system packages.

### Finish installation

- When the installation completes, a message appears:
  **“Installation Complete. You need to restart the computer to use the new system.”**
- Click **Restart Now**.
- Remove the installation media (USB/DVD) when prompted.

### First boot

- After rebooting, the computer starts from the hard drive.
- Enter your **username** and **password**.
- You are now logged in to your new Linux system.

## Post-installation setup

After installing Linux, there are a few essential steps to configure your computer for daily use. This section guides you through the most important tasks.

### First boot

1. Remove the installation media (USB/DVD) and restart the computer.
2. At the login screen, enter the **username** and **password** you created during installation.
3. Once logged in, you will see your Linux desktop for the first time.

### Update your system

Keeping your system up to date is important for security and performance.

- Open the **Terminal** from the applications menu.
- Run the update command for your distribution:

  - **Ubuntu/Debian-based:**
    ```bash
    sudo apt update && sudo apt upgrade -y  # Updates package list and upgrades installed packages
    ```
  - **Fedora:**
    ```bash
    sudo dnf update -y  # Updates installed packages
    ```
  - **Arch Linux:**
    ```bash
    sudo pacman -Syu  # Synchronizes packages and upgrades the system
    ```
- Wait for updates to finish and restart if prompted.

### Install additional drivers

Some hardware, like graphics cards or Wi-Fi adapters, may require proprietary drivers.

- Go to **Settings > Additional Drivers** (on Ubuntu and similar distributions).
- Review available drivers and install the recommended options.
- Restart the computer after installation.

### Install essential software

Linux distributions come with many applications pre-installed, but you may want additional tools for daily use.

- Some common software are:

  - **Web browsers:** Firefox, Chromium
  - **Office suite:** LibreOffice
  - **Media players:** VLC
  - **Code editors:** VS Code, gedit

- Install software using the **Software Center** (graphical app store) or the terminal.

### Configure system settings

Personalize your system to suit your preferences.

- **Time & Date:** Make sure your region and time zone are correct.
- **Display:** Adjust resolution and scaling for your monitor.
- **Appearance:** Change wallpaper, themes, and icons.
- **Keyboard shortcuts:** Customize shortcuts for efficiency.

### Enable security features

Linux is secure by default, but enabling extra protection is recommended.

1. Turn on the firewall:
```bash
  sudo ufw enable.
```
This enables the firewall to protect your system.

## Key Terms

The key and terms are listed in the following table:

| Term | Description |
|------|-------------|
| **Operating system (OS)** | The main software that manages computer hardware and software resources. It also provides a platform for running applications such as Linux, Windows, and macOS. |
| **CPU (central processing unit)** | The main processor that carries out instructions and calculations. It affects the overall speed of the system. |
| **Memory (RAM)** | Temporary storage used to hold data and applications that are currently in use. More RAM allows smoother multitasking and faster performance. |
| **Storage (HDD or SSD)** | Permanent storage where the operating system, files, and applications are saved. |
| **User interface** | The way users interact with the computer, such as through graphical desktops, icons, menus, or the command line. |
| **File** | A collection of data stored on a computer, such as a document, image, or program. |
| **File management** | The process of organizing, storing, and accessing files. Linux provides tools such as file managers and terminal commands for this purpose. |
| **Application (program)** | Software designed to perform specific tasks, such as web browsing, media playback, or document editing. |
| **Firewall** | A security feature that controls incoming and outgoing network traffic to protect the system from unauthorized access. |
| **Permissions** | Rules that define which users can read, modify, or run files and applications. Linux uses a strong permission system for security. |
| **Desktop** | The graphical workspace that lets users interact with applications, windows, and files. |
| **Command line** | A text-based interface where users type commands to interact with the operating system. It is powerful for advanced tasks and system management. |
| **Distribution (distro)** | A complete version of Linux that combines the Linux kernel with system tools, libraries, and applications (examples: Ubuntu, Fedora, Debian). |
| **ISO file** | A single file that contains a complete image of a Linux operating system. It is used to create bootable installation media. |
| **Bootable USB drive** | A USB flash drive prepared with a Linux ISO file that lets the computer start (boot) the installation process. |
| **Bootloader (GRUB)** | A program that loads the operating system when the computer starts. GRUB is the most common Linux bootloader and also supports dual-boot setups. |
| **Partition** | A division of a hard drive into sections for storing operating systems and files. |
| **Swap space** | A partition or file used as virtual memory when the system runs out of physical RAM. |
| **Checksum** | A code (such as SHA256) used to verify the integrity of a downloaded ISO file and ensure it is not corrupted. |

| **Package manager** | A tool for installing, updating, and removing software in Linux distributions (examples: `apt` for Ubuntu, `dnf` for Fedora, `pacman` for Arch).|
