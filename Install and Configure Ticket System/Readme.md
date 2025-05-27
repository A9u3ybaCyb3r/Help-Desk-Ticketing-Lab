# 🐳 Peppermint Ticketing System – Dockerized Help Desk Setup on Ubuntu

Welcome to your all-in-one guide to **deploying and configuring Peppermint**, an open-source ticketing system, using Docker on Ubuntu. Perfect for practicing real-world IT and DevOps workflows! 🧊

---

## 📚 Table of Contents

* [🧰 Requirements](#-requirements)
* [📦 Step 1: Install Docker + Docker Compose](#-step-1-install-docker--docker-compose)
* [🍃 Step 2: Prepare for Peppermint Installation](#-step-2-prepare-for-peppermint-installation)
* [🧾 Step 3: Create the Docker Compose File](#-step-3-create-the-docker-compose-file)
* [🚀 Step 4: Deploy Peppermint with Docker Compose](#-step-4-deploy-peppermint-with-docker-compose)
* [🌐 Step 5: Access the Web Interface](#-step-5-access-the-web-interface)
* [🛑 Step 6: Shut Down the App](#-step-6-shut-down-the-app)
* [🧼 Optional Docker Tips](#-optional-docker-tips)
* [🛠️ Peppermint Configuration Guide (Admin Setup & Client Creation)](#️-peppermint-configuration-guide-admin-setup--client-creation)

  * [🔁 Relaunch Peppermint (if needed)](#-relaunch-peppermint-if-needed)
  * [🔐 Step 1: Login as Admin](#-step-1-login-as-admin)
  * [👥 Step 2: Add Users](#-step-2-add-users)
  * [👤 Step 3: Add Clients](#-step-3-add-clients)
  * [🌐 Step 4: Explore Portals](#-step-4-explore-portals)
  * [🧠 Step 5: Advanced Admin Features](#-step-5-advanced-admin-features)
  * [📤 Step 6: Graceful Shutdown](#-step-6-graceful-shutdown)

---

## 🧰 Requirements

* ✅ Ubuntu machine (VM or physical)
* ✅ Terminal access with `sudo` privileges
* ✅ Stable internet connection

---

## 📦 Step 1: Install Docker + Docker Compose

📖 Follow Docker’s official installation docs:
👉 [https://docs.docker.com/engine/install/ubuntu](https://docs.docker.com/engine/install/ubuntu)

### 🔧 Clean Up Old Versions (if any)

```bash
sudo apt-get remove docker docker-engine docker.io containerd runc
```

### 🧾 Set Up Docker's Official Repository

Follow the steps in the official guide to add the GPG key and set up the Docker APT repo.

### 🧾 Set Up the Repository

![image](https://github.com/user-attachments/assets/1fb28edc-b2fa-437a-bfaa-904daba0e19a)

![image](https://github.com/user-attachments/assets/1fe583e3-3897-4e01-ae35-f60a94aec136)

### 📥 Install Docker Engine + Compose

Once the repository is ready:

![image](https://github.com/user-attachments/assets/9ce30126-a5af-494b-b3d9-a7f6bf61ddd4)

```bash
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin
```

### ✅ Test Docker Installation

![image](https://github.com/user-attachments/assets/bb92c0c6-ac36-4f5d-8532-fab90e00c7b4)

```bash
sudo docker run hello-world
```

🎉 You should see: `Hello from Docker!`

---

## 🍃 Step 2: Prepare for Peppermint Installation

🌐 Official site: [https://peppermint.sh](https://peppermint.sh)
🔧 GitHub repo: [https://github.com/Peppermint-Lab/peppermint](https://github.com/Peppermint-Lab/peppermint)

### 📂 Set Up Your Working Directory

```bash
mkdir ~/Peppermint
cd ~/Peppermint
```

![image](https://github.com/user-attachments/assets/3204c601-bdf3-4ca3-b13b-1831f78c239b)

---

## 🧾 Step 3: Create the Docker Compose File

Create `docker-compose.yml`:

Install mousepad then run it.

```bash
sudo apt install mousepad
```

```bash
mousepad docker-compose.yml
```

Paste the contents from Peppermint's GitHub `docker-compose` sample and **update**:

![image](https://github.com/user-attachments/assets/d8a792aa-0b7d-43c4-a2f9-89ccff8998e8)

![image](https://github.com/user-attachments/assets/b560bff6-012c-4e35-ae7c-ddd6762b6d34)

Save the file:

![image](https://github.com/user-attachments/assets/6f43b104-78e9-4759-93cb-bd9d73f1227c)

🔍 Double-check:

```bash
cat docker-compose.yml
```

![image](https://github.com/user-attachments/assets/dccbe0b6-dc0a-4fff-a532-00e8bae6a6f4)

---

## 🚀 Step 4: Deploy Peppermint with Docker Compose

Start the containers:

```bash
sudo docker compose up
```

![image](https://github.com/user-attachments/assets/b8371ddc-90fd-46ef-b428-5c9d694d0df4)

📥 This downloads the necessary images and starts the app.
🕐 The first launch might take a few minutes.

---

## 🌐 Step 5: Access the Web Interface

Open a browser and go to:

```
http://localhost:3000
```

### 👤 Default Admin Login:

* **Email:** `admin@admin.com`
* **Password:** `1234`

![image](https://github.com/user-attachments/assets/80aa3162-2ee1-47ec-a2b3-138febf1dd68)

You should land on the main dashboard! 📊

![image](https://github.com/user-attachments/assets/2b41249b-515d-4e8a-b5ff-8aa93c66efb8)

---

## 🛑 Step 6: Shut Down the App

To stop Peppermint:

```bash
sudo docker compose down
```

💡 If you run into issues, restart it cleanly:

```bash
sudo docker compose down && sudo docker compose up -d
```

---

## 🧼 Optional Docker Tips

* View running containers:

  ```bash
  docker ps
  ```
* Check container logs:

  ```bash
  docker logs <container_id>
  ```
* Clean unused resources:

  ```bash
  docker system prune
  ```

---

# 🛠️ Peppermint Configuration Guide (Admin Setup & Client Creation)

Now that Peppermint is live, let’s dive into configuration. This simulates tasks of an IT admin or help desk lead. 💼

---

## 🔁 Relaunch Peppermint (if needed)

If your VM was shut down:

```bash
cd ~/Peppermint
sudo docker compose down
sudo docker compose up -d
```

---

## 🔐 Step 1: Login as Admin

Access the dashboard:

```
http://localhost:3000
```

Login with:

* **Email:** `admin@admin.com`
* **Password:** `1234`

---

## 👥 Step 2: Add Users

1. Go to **Admin Settings ⚙️**

![image](https://github.com/user-attachments/assets/2971211d-a519-4e60-b93f-3c3c346cd963)

2. Navigate to **Users**

![image](https://github.com/user-attachments/assets/2edc5b48-87b3-4b64-a320-0b66785a4aa8)

3. Click **New User ➕**

![image](https://github.com/user-attachments/assets/18d0e8ea-26ce-4c95-b0cf-f88937e62b95)

4. Add:

| Name     | Email                                             | Password | Role |
| -------- | ------------------------------------------------- | -------- | ---- |
| Jared    | [jared@jared.com](mailto:jared@jared.com)         | jared    | User |
| Jin Yang | [jinyang@jinyang.com](mailto:jinyang@jinyang.com) | jinyang  | User |
| Richard  | [richard@richard.com](mailto:richard@richard.com) | richard  | User |

![image](https://github.com/user-attachments/assets/f5ddbcf8-5a0f-44eb-8af9-a8f7155b04b1)

![image](https://github.com/user-attachments/assets/552c93f0-321c-46ef-8e22-7379ad4d24ba)

📌 Tip: You can add more admins and delete the default account later.

---

## 👤 Step 3: Add Clients

1. Click **Clients** in the sidebar

![image](https://github.com/user-attachments/assets/ed84ca61-3903-4c6b-aa40-170b49e4713d)

2. Click **New Client ➕**

![image](https://github.com/user-attachments/assets/e8d90d75-1f9f-48ed-86f9-ac798c5a4728)

3. Add:

| Name   | Email                                         | Phone |
| ------ | --------------------------------------------- | ----- |
| Monica | [monica@monica.com](mailto:monica@monica.com) | 1234  |
| Gavin  | [gavin@gavin.com](mailto:gavin@gavin.com)     | 1234  |
| Peter  | [peter@peter.com](mailto:peter@peter.com)     | 1234  |

![image](https://github.com/user-attachments/assets/51dbc87d-85a3-41bc-a5d7-cff7317f6646)

![image](https://github.com/user-attachments/assets/2ed4be9a-9e2a-447c-9b87-9d34d547646f)

✅ These clients can now submit tickets.

---

## ✅ You're Ready!

You’ve now completed:

- 🚀 Deployment of Peppermint
- 👤 Admin login
- 👥 User creation
- 🙋 Client setup
- 🛠️ Admin feature overview

In the next step, you'll **log in as a regular user**, learn to **create, escalate, and resolve tickets** — just like a real help desk agent! 🧑‍💻

