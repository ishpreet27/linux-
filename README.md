# Windows Subsystem for Linux (WSL) with Ubuntu Installation Guide on Windows 11

This guide provides detailed steps to enable, install, and configure the Windows Subsystem for Linux (WSL) along with an Ubuntu distribution on Windows 11.

## Prerequisites

- Windows 11
- Administrative privileges

## Step-by-Step Instructions

### 1. Enable WSL Feature

- Open the **Control Panel**
- Navigate to **Programs and Features** > **Turn Windows features on or off**
- Check the box for **Windows Subsystem for Linux**
- Click **OK** and **restart** your computer

Alternatively, you can search for **"Turn Windows features on or off"** directly from the Windows search bar.

### 2. Verify WSL Installation

- Open **Command Prompt**
- Type `bash` and press Enter
- A message will appear stating that no Linux distributions are installed
- Follow the provided link to the Microsoft Store

### 3. Install Ubuntu from Microsoft Store

- Open the **Microsoft Store**
- Search for **Ubuntu**
- Select the general **Ubuntu** app (recommended for latest LTS version)
- Click **Get** to install

### 4. Update the WSL Kernel (If Required)

If you encounter the error:
> WSL 2 requires an update to its kernel component

Follow these steps:

- Visit the Microsoft-provided link from the error message
- Download the **WSL kernel update package** (wsl_update_x64.msi)
- Run the installer and complete the setup

### 5. Initial Ubuntu Setup

- Launch **Ubuntu** from the Start Menu
- Wait for the installation to finish
- Create a **Unix username** (does not need to match Windows)
- Set a **password** for the Unix user

### 6. Using the Ubuntu Terminal

You now have a functional Ubuntu terminal inside Windows. Try using basic commands like:

```bash
ls -al
pwd
7. Access Windows File System from Ubuntu
Windows drives are mounted under /mnt

For example:

C: drive → /mnt/c

D: drive → /mnt/d

Navigate to Desktop:

bash
Copy
Edit
cd /mnt/c/Users/<YourUsername>/Desktop
Create a file:

bash
Copy
Edit
touch test.txt
8. Alternative Access via Command Prompt
You can also access Ubuntu by typing bash in the standard Windows Command Prompt.

Benefits of Using WSL
Run Linux tools and scripts natively on Windows

Access both Windows and Linux file systems seamlessly

Avoid dual-booting or virtual machines

Ideal for developers working in cross-platform environments

Troubleshooting
Ensure Windows features are correctly enabled

Make sure your system is updated

If installation issues persist, refer to the official WSL documentation: https://docs.microsoft.com/windows/wsl

