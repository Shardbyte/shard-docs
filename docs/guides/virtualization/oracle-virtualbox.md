---
title: Oracle VirtualBox
---

<figure markdown>
  ![Image title](https://shardbyte.com/assets/images/guides/virtualbox/virtualbox-image-001.webp){ width="580" }
  <figcaption>VirtualBox</figcaption>
</figure>

# **VirtualBox**
VirtualBox is a powerful virtualization tool that allows you to run multiple operating systems on a single computer. Whether you want to test software, experiment with different operating systems, or create virtual development environments, VirtualBox is a valuable tool. This step-by-step guide will walk you through the process of setting up VirtualBox on your computer.

### **Step 1: Download VirtualBox**

1. Go to the VirtualBox website: [VirtualBox Website](https://www.virtualbox.org/).
2. On the VirtualBox website's main page, you'll see a prominent "Downloads" section. Click on this section to proceed.

!!! note
    After clicking on the "Downloads" section, you'll be taken to a page where you can choose the version of VirtualBox that's suitable for your operating system (Windows, macOS, Linux, etc.). Follow these steps:

##### **Choose Download Version:**
  - Click on the version that matches your host operating system. For example, if you're using Windows, click on the Windows version.

##### **Download in Progress:**
  - Wait for the download to complete. The time it takes depends on your internet connection speed.

### **Step 2: Install VirtualBox**

##### **Locate the Downloaded Installation File:**
  - After downloading the VirtualBox installation file, you need to locate it in your computer's download directory. By default, most browsers save downloaded files in the "Downloads" folder.

##### **Run the Installation File:**
  - Double-click on the downloaded VirtualBox installation file. The file will typically have a name like `VirtualBox-x.x.x-Installer.exe` (1)
{ .annotate }

1.  (where "x.x.x" represents the version number)

##### **User Account Control (UAC) Prompt (Windows):**
  - On Windows, the User Account Control (UAC) prompt may appear. If it does, click "Yes" to allow the installation to proceed.

##### **VirtualBox Setup Wizard:**
  - The VirtualBox Setup Wizard will open. Click "Next" to begin the installation process.

##### **Choose Components:**
  - You'll be asked to select the components you want to install. By default, VirtualBox and Oracle VM VirtualBox Extension Pack are selected. We recommend installing both components, so leave these options as they are.

##### **Choose Install Location:**
  - Specify the folder where you want VirtualBox to be installed. The default location is usually in the "C:\Program Files\Oracle\VirtualBox" directory. You can change this location if needed by clicking the "Browse" button.

##### **Warning About Network Interfaces (Windows):**
  - If you're using Windows, you might see a warning about network interfaces during the installation. This is related to VirtualBox's network setup. Click "Yes" to proceed.

##### **Create Start Menu Shortcuts:**
  - Choose whether you want to create shortcuts in the Start Menu. By default, both options ("Create shortcuts on the desktop" and "Create shortcuts in the Start Menu") are selected. You can uncheck them if you prefer not to have shortcuts.

##### **Ready to Install:**
  - Review your installation settings on the summary screen. If everything looks correct, click "Install" to start the installation.

##### **Installation Progress:**
  - The installer will copy files and install VirtualBox on your computer. This process may take a few minutes.

##### **Installation Complete:**
  - Once the installation is complete, you'll see a "Completing the Oracle VM VirtualBox Setup Wizard" screen. Make sure the "Start Oracle VM VirtualBox after installation" option is checked. Click "Finish."

##### **VirtualBox Installed:**
  - Oracle VM VirtualBox is now installed on your computer and should open automatically. You can also find it in your Start Menu or desktop, depending on the options you selected.

### **Step 3: Create a Virtual Machine**

!!! note
    Creating a virtual machine in VirtualBox is a crucial step that involves configuring the virtual hardware and settings for the guest operating system you want to run. Here's a more in-depth look at this step:

##### **Open VirtualBox:**
  - After installing VirtualBox, open the application.

##### **Click "New":**
  - In the VirtualBox Manager, click the "New" button to initiate the creation of a new virtual machine.

##### **Name and Operating System Type:**
1. In the "Name" field, give your virtual machine a descriptive name.
2. In the "Machine Folder" field, you can specify the folder where the virtual machine files will be stored.
3. Select the "Type" of the operating system you plan to install. This could be Windows, Linux, macOS, or another OS. VirtualBox will preconfigure some settings based on your selection.

##### **Choose the Operating System Version:**
  - In the "Version" dropdown, select the specific version or distribution of the operating system. If your OS version isn't listed, choose the one that's closest to it.

##### **Memory (RAM) Allocation:**
  - Specify the amount of memory (RAM) to allocate to the virtual machine. The amount you allocate depends on the requirements of the guest OS and the available resources on your host computer.

##### **Create a Virtual Hard Disk:**
1. Select "Create a virtual hard disk now" and click "Create."
2. You'll be guided through the Virtual Hard Disk Creation Wizard. Here, you can choose the file type (typically VDI for VirtualBox), allocate the size of the virtual hard disk, and choose whether it should be dynamically allocated (which is more space-efficient) or fixed size.

##### **Hard Disk File Location and Size:**
1. Choose where you want to save the virtual hard disk file on your host computer.
2. Set the size of the virtual hard disk. This size should provide enough space for the guest OS and its software.

##### **Review and Create:**
1. Review your settings on the summary page to ensure they are correct.
2. Click "Create" to finish creating the virtual machine.

##### **Virtual Machine Created:**
  - Once you click "Create," your virtual machine will be created and listed in the VirtualBox Manager.

!!! note
    Your virtual machine is now set up and almost ready for the installation of the guest operating system. You can return to the VirtualBox Manager to start the installation process as described in Step 4.
### **Step 4: Download Fedora 38 Workstation**

!!! note
    Downloading the Fedora 38 Workstation ISO file is the first step to installing it in a VirtualBox virtual machine. Follow these steps:

##### **Visit the Official Fedora Website:**
  - Open your web browser and go to the official Fedora website at [Get Fedora](https://getfedora.org/).

##### **Select the Workstation Edition:**
  - On the Fedora website, you'll see different editions of Fedora. Click on the "Workstation" edition. This is the version suitable for desktop use and general purposes.

##### **Choose Your Download Option:**
1. You'll be presented with options for downloading Fedora 38 Workstation. Typically, there's a direct download link.
2. Click on the link to download the ISO file. This file is relatively large, so it may take some time to complete the download.

##### **Verify Your Download (Optional):**
  - To ensure the integrity of your download, you can verify the downloaded ISO file's checksum using the provided checksums on the Fedora website.

##### **Download in Progress:**
  - Wait for the download to complete. The time it takes depends on your internet connection speed.

##### **ISO File Ready:**
  - Once the download is finished, you'll have the Fedora 38 Workstation ISO file ready to use for the installation process in VirtualBox.

### **Step 5: Install Fedora 38 Workstation in VirtualBox**

!!! note
    Installing the Fedora 38 Workstation in a VirtualBox virtual machine allows you to explore the latest features and applications of this Linux distribution.

##### **Create or Open Your Virtual Machine:**
  - Open VirtualBox and select your previously created virtual machine.

##### **Select Fedora ISO:**
1. In the VirtualBox Manager, make sure your virtual machine is selected.
2. Click the "Settings" button.
3. In the "Storage" section, under "Controller: IDE," select the empty CD/DVD icon.
4. In the attributes section, click the CD/DVD icon next to "Optical Drive."
5. Choose "Choose a disk file" and select the Fedora 38 Workstation ISO file you downloaded in Step 1.
6. Click "OK" to save the settings.

##### **Start the Virtual Machine:**
  - In the VirtualBox Manager, select your virtual machine and click "Start."

##### **Begin the Fedora Installation:**
1. Your virtual machine should boot from the Fedora ISO you provided.
2. Select "Start Fedora Workstation Live" and press Enter.

##### **Fedora Live Environment:**
  - You will be presented with the Fedora Live environment. You can explore Fedora without making any changes to your system.

##### **Start Installation:**
  - Double-click the "Install to Hard Drive" icon on the desktop to begin the installation.

##### **Choose Language and Keyboard Layout:**
  - Select your language and keyboard layout.

##### **Set Root Password:**
  - Create a root password for the system.

##### **Create a User:**
  - Set up a user account by providing a username and password.

##### **Installation Summary:**
  - Configure your installation settings, including the installation destination and network configuration. Click "Begin Installation" when ready.

##### **Installation Progress:**
  - Fedora 38 Workstation will be installed on your virtual machine. This may take some time.

##### **Complete Installation:**
  - After the installation is complete, click "Quit" to exit the installer.

##### **Shutdown Your Virtual Machine:**
  - Shutdown your virtual machine.

##### **Remove Fedora ISO:**
1. In the VirtualBox Manager, make sure your virtual machine is selected.
2. Click the "Settings" button.
3. In the "Storage Devices" section, you will see the ISO file listed under "Controller: IDE" or "Controller: SATA." It will be in the Optical Drives subsection, select the ISO file by clicking on it to highlight it.
4. Once the ISO file is selected, click on the small disk icon with the red minus ("-") sign at the top of the Storage Devices list. This icon represents "Remove Attachment."
5. Click "OK" to save the settings.

!!! success
    Enjoy exploring and using Fedora 38 Workstation within your VirtualBox environment!

### **Step 6: Start and Use Your Virtual Machine**

1. In VirtualBox, select your virtual machine and click "Start."
2. Your virtual machine will boot, and you can use it just like a physical computer.
3. You can switch between your host and virtual machine by using keyboard shortcuts (e.g., Right Ctrl on Windows).

!!! warning
    Remember that the virtual hardware settings, such as the number of CPU cores, graphics memory, and network configuration, can be adjusted in the virtual machine's settings, which we mentioned in Step 3. These settings can be fine-tuned to match the requirements of your guest OS and any specific needs you might have for your virtual environment.

### **Conclusion**
Setting up VirtualBox can be a valuable addition to your computing environment. It allows you to run multiple operating systems concurrently, making it an excellent tool for various purposes. Whether you're a developer, tester, or simply curious about different operating systems, VirtualBox offers flexibility and convenience.
