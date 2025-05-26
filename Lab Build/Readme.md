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

![image](https://github.com/user-attachments/assets/ce589cd0-4f47-4a3c-93ab-64770ace74fd)

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

![image](https://github.com/user-attachments/assets/420ca717-101d-47d5-95f5-deb8d8a33625)

2. 🧾 Name your VM (e.g., `Ubuntu-PhD`)
3. 📂 Choose a folder for your VM files (optional)
4. 🗂️ Select **"Other"** to browse and choose the Ubuntu ISO you downloaded
5. 🧪 **Uncheck "Skip Unattended Installation"**  
    → This lets you walk through the manual install steps

![image](https://github.com/user-attachments/assets/3e658fa4-b8fb-4a68-8978-3338c48ded33)

---

## 🧠 3. Allocate System Resources

Make sure your host system has enough resources!  

![image](https://github.com/user-attachments/assets/867f916d-124a-47cb-b7d0-03029cd8dbc9)

Set these according to your PC’s specs:

- 🧠 **RAM**:
    
    - 16GB system: allocate **8GB** (8192 MB)
    - 8GB system: allocate **4GB**

- 🧮 **CPU Cores**:
    
    - Allocate **2 to 6 cores**, staying in the **green** range

🟢 Staying in the green ensures your host OS won't suffer performance issues.

---

## 💽 4. Create Virtual Hard Disk

![image](https://github.com/user-attachments/assets/525577e6-74b1-4932-bc9d-6581b3a0d506)

- Minimum: **25 GB**
- Recommended: **50 GB**

🗂️ Click **Next** and **Finish** when you're happy with the settings.

Now your VM is created, but it’s still powered off.

---

## 🚀 5. Start the Installation

1. ⚡ Click **Start** in VirtualBox
2. 📺 Wait a few moments while it boots
3. 🖱️ Choose **Try or Install Ubuntu**
4. Click **Install Ubuntu** if it prompts you to.

![image](https://github.com/user-attachments/assets/219ac249-1915-4fcf-a3d2-4dfb0d2ef806)

---

## 🛠️ 6. Walk Through Ubuntu Installer

### 🧭 Setup Steps:

- 🌐 Language: Select **English** or your preferred language

![image](https://github.com/user-attachments/assets/40b4a4e4-e630-4a6b-ac58-3d2b0a3c8371)

- 🖥️ Keyboard: Default is **English (US)**

![image](https://github.com/user-attachments/assets/c90017ea-03d6-4d30-bdf9-67f48a186079)

- 🌐 Internet: Choose **Wired Connection** (even if you're on Wi-Fi)

![image](https://github.com/user-attachments/assets/10c150ef-4782-4262-928a-904ab6d2e837)

- 💻 Installation Type: **Normal Installation**

![image](https://github.com/user-attachments/assets/04270b6c-9c52-4290-ab30-8d001e49f64c)

![image](https://github.com/user-attachments/assets/149bac0b-6739-4d01-b6f8-04065dfb8a02)

![image](https://github.com/user-attachments/assets/efad9cf2-c57a-4b8f-a365-d184fb1947ee)

- 📦 Select **Install third-party software** for drivers

![image](https://github.com/user-attachments/assets/48c20caa-64cf-4c20-9616-70eaf5987555)

- 📀 Storage: Choose **Erase Disk and Install Ubuntu** (safe for VM)

![image](https://github.com/user-attachments/assets/fb6c3608-46d8-4c10-8cd0-9049152c06f6)

---

## 👤 7. User Setup

Fill in your details:

- **Name**: e.g., Andrew
- **Computer Name**: e.g., Andrew-Ubuntu-PhD
- **Username**: your preferred username
- **Password**: choose one (e.g., `password` for easy recall—but use something secure in real life!)

![image](https://github.com/user-attachments/assets/27f1af51-5a12-4405-8f1b-6db643e3a8b6)

🕒 Choose your **time zone**  

![image](https://github.com/user-attachments/assets/54e8847b-e64f-4185-8070-8e6f69d106b6)

🔁 Click **Install** and let it complete (this will take a few minutes)

![image](https://github.com/user-attachments/assets/900d9e54-87a6-48ac-9356-16277734d1d0)

---

## 🔄 8. Restart and Finalize Setup

1. 🌀 Click **Restart Now**

![image](https://github.com/user-attachments/assets/099b3c69-300c-4897-9d57-4686971d076f)

2. 🔐 Log in using your password

![image](https://github.com/user-attachments/assets/e6f28dd0-5906-4b09-8412-2a5a53ae5e85)

3. 🧹 Skip the **Ubuntu Pro** subscription

![image](https://github.com/user-attachments/assets/9af28543-fc9f-4334-9548-f73be41ef19e)

![image](https://github.com/user-attachments/assets/348baeb0-7877-4e70-b6a0-1831e873d249)

4. 📊 Select **Don’t share system data**

![image](https://github.com/user-attachments/assets/35d368bb-db4f-45a3-8350-0d25324fe7e4)

5. ✅ Click **Finish**

🎉 Congrats! Your Ubuntu virtual machine is ready to use!

---

# 🧰 Ubuntu VM Post-Install Setup & UI Walkthrough

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

---

## 🎉 You’re Ready to Explore Ubuntu!

This wraps up your **initial setup** and **desktop UI overview** for Ubuntu. Next, we are going to install Docker and Peppermint.
