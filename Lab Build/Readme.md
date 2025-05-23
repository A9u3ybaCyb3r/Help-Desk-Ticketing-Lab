# 📚 Table of Contents
1. [Download Ubuntu ISO](#-1-download-ubuntu-iso)
2. [Open VirtualBox and Create a New VM](#-2-open-virtualbox-and-create-a-new-vm)
3. [Allocate System Resources](#-3-allocate-system-resources)

---

# 🧰 How to Install Ubuntu Linux in VirtualBox

_A beginner-friendly setup guide for your first Linux virtual machine_

---

## 📥 1. Download Ubuntu ISO

👉 Head to the official website:  
🔗 [Ubuntu Download Page](https://ubuntu.com/download/desktop)

### Choose the Version:

- ✅ Select **Ubuntu 24.04 LTS (Long Term Support)**  
    ⏳ _Get 5 years of security & software updates!_
![[Pasted image 20250522142023.png]]
1. Click **Download Ubuntu Desktop**
2. Ignore the newsletter prompt, and the ISO download will begin automatically
3. Save the `.iso` file to your **Desktop** or a preferred folder
![[Pasted image 20250522142000.png]]
📁 _The ISO file is a virtual disc image that contains the OS installer._

---

## 🖥️ 2. Open VirtualBox and Create a New VM

Download & install [VirtualBox](https://www.virtualbox.org/) if you haven’t already.

### Steps in VirtualBox:

1. 🔧 Click **Machine > New**
![[Pasted image 20250522142106.png]]
2. 🧾 Name your VM (e.g., `Ubuntu-PhD`)
3. 📂 Choose a folder for your VM files (optional)
4. 🗂️ Select **"Other"** to browse and choose the Ubuntu ISO you downloaded
5. 🧪 **Uncheck "Skip Unattended Installation"**  
    → This lets you walk through the manual install steps
![[Pasted image 20250522142133.png]]

---

## 🧠 3. Allocate System Resources

Make sure your host system has enough resources!  
![[Pasted image 20250522142218.png]]
Set these according to your PC’s specs:

- 🧠 **RAM**:
    
    - 16GB system: allocate **8GB** (8192 MB)
    - 8GB system: allocate **4GB**

- 🧮 **CPU Cores**:
    
    - Allocate **2 to 6 cores**, staying in the **green** range

🟢 Staying in the green ensures your host OS won't suffer performance issues.

---

## 💽 4. Create Virtual Hard Disk
![[Pasted image 20250522143245.png]]
- Minimum: **25 GB**
- Recommended: **50 GB**

🗂️ Click **Next** and **Finish** when you're happy with the settings.

Now your VM is created, but it’s still powered off.

---

## 🚀 5. Start the Installation

1. ⚡ Click **Start** in VirtualBox
2. 📺 Wait a few moments while it boots
3. 🖱️ Choose **Try or Install Ubuntu**
4. Click **Install Ubuntu**
![[Pasted image 20250522143314.png]]
![[Pasted image 20250522143346.png]]

---

## 🛠️ 6. Walk Through Ubuntu Installer

### 🧭 Setup Steps:

- 🌐 Language: Select **English** or your preferred language
![[Pasted image 20250522143404.png]]
- 🖥️ Keyboard: Default is **English (US)**
![[Pasted image 20250522143426.png]]
- 🌐 Internet: Choose **Wired Connection** (even if you're on Wi-Fi)
![[Pasted image 20250522143817.png]]
- 💻 Installation Type: **Normal Installation**
![[Pasted image 20250522144301.png]]
![[Pasted image 20250522144313.png]]
![[Pasted image 20250522144326.png]]
- 📦 Select **Install third-party software** for drivers
![[Pasted image 20250522144400.png]]
- 📀 Storage: Choose **Erase Disk and Install Ubuntu** (safe for VM)
![[Pasted image 20250522144411.png]]

---

## 👤 7. User Setup

Fill in your details:

- **Name**: e.g., Andrew
- **Computer Name**: e.g., Andrew-Ubuntu-PhD
- **Username**: your preferred username
- **Password**: choose one (e.g., `password` for easy recall—but use something secure in real life!)
![[Pasted image 20250522144431.png]]

🕒 Choose your **time zone**  
![[Pasted image 20250522144446.png]]
🔁 Click **Install** and let it complete (this will take a few minutes)
![[Pasted image 20250522144504.png]]

---

## 🔄 8. Restart and Finalize Setup

1. 🌀 Click **Restart Now**
![[Pasted image 20250522144948.png]]
2. 🔐 Log in using your password
![[Pasted image 20250522145001.png]]
3. 🧹 Skip the **Ubuntu Pro** subscription
![[Pasted image 20250522145032.png]]
4. 📊 Select **Don’t share system data**
![[Pasted image 20250522145017.png]]
5. ✅ Click **Finish**

🎉 Congrats! Your Ubuntu virtual machine is ready to use!

---

# 🧰 Ubuntu VM Post-Install Setup & UI Walkthrough

_A practical guide to setting up your Ubuntu Desktop VM in VirtualBox_

---

## 📸 Step 1: Take a Snapshot (Highly Recommended)

Before making any major changes to your VM:

### 🔄 Create a Snapshot

1. In VirtualBox:  
    **Machine → Take Snapshot**
![[Pasted image 20250522145636.png]]
2. Name it something like:
```
Fresh Installation
```
![[Pasted image 20250522145708.png]]
3. (Optional) Add a description like:
    > “Just installed Ubuntu. No changes made yet.”

✅ Snapshots help you **roll back** quickly if you break something.

---

## 💡 Why Snapshots Matter

- Linux offers **freedom**, but with fewer guardrails than Windows
- That means it’s easier to break something accidentally
- Snapshots act like **save points** 🕹️ for your VM

---

## 👤 Step 2: Log In & Access the Ubuntu Desktop

Once logged in, you'll see the **GNOME Desktop Environment**. GNOME is:

- 🖥️ Ubuntu's default user interface
- 📦 Shared by other Linux distros too (but not all)

---

## 🧭 Step 3: Open the App Menu

Click the **Ubuntu logo** in the bottom-left corner (similar to the Windows Start menu):
![[Pasted image 20250522145912.png]]
### From here, you can:

- 🔍 Search for and open applications
- ⚙️ Access **Settings**
- 🛒 Browse the **Ubuntu Software** store

---

## 🖥️ Step 4: Adjust Display Settings

To make the display more usable:

### Change Screen Resolution:

1. Go to **Settings**
2. Navigate to **Display**
3. Set resolution to `1920x1080` (or match your monitor)
4. Keep **Scale** at `100%`
5. Click **Apply** and confirm the changes
![[Pasted image 20250522153521.png]]

---

## 🖼️ Step 5: Full-Screen Mode in VirtualBox

Want your VM to feel like a native OS?

### Enable Full-Screen Mode:

1. Go to **View → Full-Screen Mode**
2. Or press `Right Ctrl + F` (default Host Key + F)
![[Pasted image 20250522153607.png]]
🔁 To exit full-screen mode: press the **same keys again**

📌 You may need to install **VirtualBox Guest Additions** to optimize display resizing.

---

## 🗂️ Step 6: Explore the Desktop UI

### 📂 File Explorer (Left Sidebar)
![[Pasted image 20250522153646.png]]
- Works like Windows File Explorer
- Lets you browse files and folders in your Linux file system

### 🛒 Ubuntu Software Center
![[Pasted image 20250522153730.png]]
- Install apps easily like:
    
    - 🗓️ Calendar
    - 🖌️ Paint apps
    - 🎮 Games

(You’ll learn more about app installations in a later lesson.)

---

## 🔧 Step 7: System Menu (Top-Right Corner)

Click the top-right status bar to:
![[Pasted image 20250522153746.png]]
- 🌐 Manage network settings (usually set to Wired via NAT)
- 🔒 Lock or power off the VM
- ⚙️ Access system settings

⚠️ Some UI pop-ups are from **VirtualBox**, not Ubuntu itself.
