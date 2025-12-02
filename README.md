
# Ex.3: Virtualization — Installation and Configuration of Oracle VirtualBox & Kali Linux, and Execution of Linux Commands

---

## Aim:
To set up a virtualized environment using Oracle VirtualBox, install Kali Linux as a guest operating system, and execute fundamental Linux commands in the Kali environment.

---

## 3.a) Installation and Configuration of Oracle VirtualBox

### Aim:
To install and configure Oracle VM VirtualBox.

### Prerequisites:
- Machine with Internet access  
- Minimum 4 GB RAM  
- At least 20 GB of free storage space  

### Steps:

1. **Download Oracle VirtualBox:**
   - Visit the official [Oracle VirtualBox site](https://www.virtualbox.org/)
   - Download the appropriate installer for your OS (Windows/macOS/Linux)

2. **Install VirtualBox:**
   - Launch the installer → Allow changes → Click `Next`  
   - Choose installation options → Click `Next`  
   - Accept network warning → Click `Yes`  
   - Click `Install` → Finish and launch VirtualBox

3. **Initial Configuration:**
   - Open VirtualBox  
   - Click `New` → Set a name (e.g., Kali)  
   - Choose Type: Linux → Version: Debian (64-bit)  
   - Allocate:
     - At least 2 GB RAM  
     - Create a new virtual hard disk (20 GB recommended)

---

### Result:
Oracle VM VirtualBox was successfully installed and configured.

---

## 3.b) Installation and Configuration of Kali Linux

### Aim:
To install and configure Kali Linux in Oracle VirtualBox.

### Prerequisites:
- Oracle VirtualBox installed  
- Minimum 4 GB RAM and 20 GB storage  
- Kali Linux ISO image  

### Steps:

1. **Download Kali Linux ISO:**
   - Visit the [Kali Linux official site](https://www.kali.org/)
   - Download the 64-bit ISO (Installer version)

2. **Create a New Virtual Machine:**
   - Open VirtualBox → Click `New`  
   - Name: "Kali Linux" → Type: Linux → Version: Debian (64-bit)

3. **Memory Allocation:**
   - Assign at least 2 GB RAM (4 GB recommended)

4. **Create a Virtual Hard Disk:**
   - Choose VDI (VirtualBox Disk Image)  
   - Select Dynamically allocated  
   - Set size: Minimum 20 GB

5. **Attach ISO Image:**
   - Settings → Storage → Controller: IDE → Empty → Choose Disk File → Select Kali Linux ISO

6. **Install Kali Linux:**
   - Start the VM  
   - Choose Graphical Install  
   - Set language, region, and keyboard  
   - Configure network (hostname)  
   - Set root password  
   - Disk partitioning: Use entire disk → All files in one partition  
   - Install system → Install GRUB bootloader → Finish

7. **Login:**
   - Use root credentials to log in

8. **Optional – Guest Additions:**
   - Devices → Insert Guest Additions CD Image → Follow installation instructions

---

### Snapshots:

- **Snapshot 1**: Oracle VirtualBox Installation  
  ![image](https://github.com/user-attachments/assets/737dafde-fd5d-4266-849a-a12013ce9c5b)

- **Snapshot 2**: Kali Linux Running in VirtualBox  
  ![image](https://github.com/user-attachments/assets/6b08c65e-e2c0-4f8e-a782-0914a3470759)

---

### Result:
Kali Linux guest OS was successfully installed and configured in Oracle VirtualBox.

---

## 3.c) Execution of Linux Commands in Kali

### Overview:
- Linux is an open-source OS where the kernel manages system resources.
- Command-line interaction is powerful and essential for system administration.
- All Linux commands are case-sensitive.

---

### Executed Commands:

| S.No | Command | Description | Syntax | Screenshot |
|------|---------|-------------|--------|------------|
| 1 | `ls` | List directory contents | `ls` | ![ls](https://github.com/user-attachments/assets/515d3f10-a956-46cd-9abb-cc078c9b5a34) |
| 2 | `pwd` | Print working directory | `pwd` | ![pwd](https://github.com/user-attachments/assets/126560e9-81fb-4f48-b2d6-fc1c687d7923) |
| 3 | `mkdir` | Create a new directory | `mkdir <dir>` | ![mkdir](https://github.com/user-attachments/assets/faff0a46-f085-47e6-9c3e-17a0804c192c) |
| 4 | `rmdir` | Remove a directory | `rmdir <dir>` | ![rmdir](https://github.com/user-attachments/assets/645b7709-ac2a-4f69-8290-1dab26cb1654) |
| 5 | `cd` | Change directory | `cd <dir>` | ![cd](https://github.com/user-attachments/assets/11b9a3cd-93b0-4523-aaef-1b6ff79a7a72) |
| 6 | `cat` | Display file contents | `cat <file>` | ![cat](https://github.com/user-attachments/assets/44647c5d-6f0b-47e3-ae58-68a255bbf50f) |
| 7 | `cp` | Copy files | `cp <src> <dest>` | ![cp](https://github.com/user-attachments/assets/84a642ac-a208-42ec-b741-8401626414bb) |
| 8 | `gedit` | Open text editor | `gedit <file>` | ![gedit](https://github.com/user-attachments/assets/2165b336-4119-432e-aeb6-ea76f1725ff7) |
| 9 | `su` | Switch user | `su <username>` | ![su](https://github.com/user-attachments/assets/751f7f38-38f3-4046-8791-1604f6b27c0a) |
| 10 | `mv` | Move/rename files | `mv <src> <dest>` | ![mv](https://github.com/user-attachments/assets/191aeba3-450c-49de-8248-e4e5265f28ca) |
| 11 | `rename` | Rename files | `rename 's/old/new/' files` | ![rename](https://github.com/user-attachments/assets/04e837d0-09d5-4b7e-8d2f-0f0745566af9) |
| 12 | `head` | Show first 10 lines | `head <file>` | ![head](https://github.com/user-attachments/assets/bdf4d996-0e44-4f5b-ada0-150c71cfb58a) |
| 13 | `tail` | Show last 10 lines | `tail <file>` | ![tail](https://github.com/user-attachments/assets/d1abc737-da54-482a-8f3b-3208f5c0b6ec) |
| 14 | `id` | Display user/group ID | `id` | ![id](https://github.com/user-attachments/assets/c4e63382-19b1-462f-a8fb-4ac1b106c186) |
| 15 | `grep` | Search pattern in output | `grep <word>` | ![grep](https://github.com/user-attachments/assets/d5d05747-0644-4862-ba9c-9be4634eeb89) |
| 16 | `tr` | Translate characters | `tr 'a' 'A'` | ![tr](https://github.com/user-attachments/assets/111a3959-d573-48a0-bbf6-52a5b4eb52a1) |
| 17 | `chmod` | Change file permissions | `chmod 755 <file>` | ![chmod](https://github.com/user-attachments/assets/0437e7d3-9399-47ba-8de0-af2c4f44674e) |
| 18 | `tar` | Archive files | `tar -xvzf file.tar` | ![tar](https://github.com/user-attachments/assets/0faa99fa-f1ad-45f9-a95d-aeded05b2520) |
| 19 | `chown` | Change file ownership | `chown user file` | ![chown](https://github.com/user-attachments/assets/e47392dd-f5bf-41c7-b95c-79245763ecc1) |
| 20 | `make` | Build/compile programs | `make` | ![make](https://github.com/user-attachments/assets/d330e936-84f4-4e94-a206-1659319727fa) |
| 21 | `ifconfig` | Display network config | `ifconfig` | ![ifconfig](https://github.com/user-attachments/assets/0042ccf4-9647-4bb3-bcdd-3c9e169b3a0c) |
| 22 | `chmod 777` | Full access permissions | `chmod 777 <file>` | ![chmod777](https://github.com/user-attachments/assets/9781ab44-ee9c-4416-ac6d-0e11be392364) |
| 23 | `host` | DNS lookup | `host <domain>` | ![host](https://github.com/user-attachments/assets/f51d6c24-79c7-4fcc-a2d2-4c34b3b18a83) |
| 24 | `gzip` | Compress files | `gzip <file>` | ![gzip](https://github.com/user-attachments/assets/0b474ac8-f2d6-4360-a753-8d897c72a68f) |
| 25 | `sort` | Sort file contents | `sort <file>` | ![sort](https://github.com/user-attachments/assets/8f9dbc43-e32b-4b44-9f3d-bae35ba8b62b) |
| 26 | `cal` | Show calendar | `cal` | ![cal](https://github.com/user-attachments/assets/8e6db122-78d3-4034-a339-04d623308630) |
| 27 | `clear` | Clear terminal | `clear` | ![clear](https://github.com/user-attachments/assets/bce65060-aeea-4469-89fa-8ea90cdb5d24) |
| 28 | `mail` | Send emails | `mail -s "Subject" <recipient>` | ![mail](https://github.com/user-attachments/assets/54599c39-b774-49b0-8046-ecb6334019dd) |
| 29 | `df` | Disk space usage | `df` | ![df](https://github.com/user-attachments/assets/316f4eac-e920-4843-8a48-924e9cfc4d47) |
| 30 | `find` | Locate files | `find . -name "*.pdf"` | ![find](https://github.com/user-attachments/assets/106fcb32-447f-4c14-acc8-a0d72c2f40dd) |

---

### Result:
The installation and configuration of Oracle VirtualBox and Kali Linux were completed successfully. Furthermore, all 30 essential Linux commands were executed in the Kali environment, enhancing command-line proficiency.
