
# 🎟️ Peppermint Help Desk User Guide: Ticket Creation, Assignment & Resolution

Welcome to Part 3 of the Peppermint ticketing lab! 🚀
In this guide, you'll step into the shoes of a **help desk technician**, working with real-world ticket flows:
📝 Creating tickets → 💬 Commenting → ♻️ Reassigning → ✅ Closing them.

---

## 📋 Table of Contents

* [🔐 Step 0: Log in as a Regular User](#-step-0-log-in-as-a-regular-user)
* [🆕 Step 1: Create a New Ticket](#-step-1-create-a-new-ticket)
* [💬 Step 2: Add Comments to a Ticket](#-step-2-add-comments-to-a-ticket)
* [🌐 Step 3: Create Another Ticket with Escalation](#-step-3-create-another-ticket-with-escalation)
* [♻️ Step 4: Escalate & Reassign the Ticket](#-step-4-escalate--reassign-the-ticket)
* [🚦 Step 5: Update Ticket Priority & Status](#-step-5-update-ticket-priority--status)
* [✅ Step 6: Resolve and Close the Ticket](#-step-6-resolve-and-close-the-ticket)
* [🧠 Key Takeaways](#-key-takeaways)
* [⚠️ Peppermint Ticket Interrupt Lab: Layered Troubleshooting & Escalation](#-peppermint-ticket-interrupt-lab-layered-troubleshooting--escalation)

  * [🔧 Scenario Summary](#-scenario-summary)
  * [🔍 Diagnostic Questions](#-diagnostic-questions)
  * [🔧 Layer 1–3 Troubleshooting](#-layer-13-troubleshooting)
  * [📋 Internal Comment Example](#-internal-comment-example)
  * [♻️ Reassign the Ticket](#-reassign-the-ticket)
  * [🧠 Why This Matters](#-why-this-matters)
  * [🎉 Success!](#-success)

---

## 🔐 Step 0: Log in as a Regular User

1. Open your browser to:

```
http://localhost:3000
```

2. Click **Logout** from the admin account if you're still logged in.

![image](https://github.com/user-attachments/assets/2a0d1ead-7c76-404f-85be-6d1c4997b193)

3. Sign in with a non-admin user (like Jared):

   * **Email:** `jared@jared.com`
   * **Password:** `jared`

---

## 🆕 Step 1: Create a New Ticket

1. On the left sidebar, click **Create Ticket ➕**

![image](https://github.com/user-attachments/assets/d323ccfe-b9ba-49fb-a847-a3b421b04c03)

2. Fill out the form:

| Field       | Value                                                      |
| ----------- | ---------------------------------------------------------- |
| Title       | Need Help Installing Outlook                               |
| Description | Hello Help Desk, could you please help me install Outlook? |
| Client      | Monica                                                     |
| Engineer    | Jared (yourself)                                           |
| Type        | Feature Request                                            |

![image](https://github.com/user-attachments/assets/0707e799-be9b-4734-858c-2e459c4f7180)

3. Click **Create Ticket ✅**
4. Navigate to **Jared's Open Tickets** to view it.

![image](https://github.com/user-attachments/assets/4dcc00d8-0ad6-4a82-9cf1-b2218047395d)

---

## 💬 Step 2: Add Comments to a Ticket

1. Click on the ticket.
2. Scroll to the **Comments** section.
3. Add a comment like:

### 🧾 Comment 1: Network Info

> 📄 _Internal Note_

```
Additional details from Monica's setup:
1. Monica is connected via Ethernet
2. Subnet: 10.0.0.0/24
3. Gateway: 10.0.0.1
```

![image](https://github.com/user-attachments/assets/4049c20e-5e40-46ba-9797-683f604d45e1)

✅ Click **Comment** (internal only)

---

### 🧪 Comment 2: Troubleshooting Steps (OSI Layers 1–3)

> 🧰 _Internal Note – Layered Troubleshooting_

---
```
Troubleshooting steps performed.
Layer 1:
- Monica verified her Ethernet cable was plugged in, no visible damage
- Link light on NIC is active

Layer 2:
- Data light flashing on NIC
- Ran `arp -a`, confirmed presence of other devices and MAC address for gateway

Layer 3:
- Successfully pinged 10.0.0.1 (gateway)
- Unable to ping www.google.com
- Ran the following:
    - ipconfig /release
    - ipconfig /flushdns
    - ipconfig /renew
    - ipconfig /registerdns
- Still no connectivity
- Trace route stops at the gateway
```

![image](https://github.com/user-attachments/assets/d1567644-b148-46ba-8443-06aa6980e70b)

✅ Click **Comment** (internal only)

---

### 🔁 Comment 3: Escalation Note

> 🧪 _Internal Note – Escalation_

```
Reached end of Help Desk Layer 3 support scope.
Escalating ticket to Tier 2 – Jin Yang for further investigation.
```

![image](https://github.com/user-attachments/assets/570718a3-797f-41b8-b48d-1f1bfbadbd7b)

✅ Click **Comment**

---

## 🔁 Step 4: Escalate the Ticket

1. Reassign the ticket to **Jin Yang**
2. Set **Priority** to `High`
3. Change status tag to **In Progress** or **Escalated**

![image](https://github.com/user-attachments/assets/248631d6-2d31-4557-b8d9-2af6e33fbeb7)

![image](https://github.com/user-attachments/assets/46aa3662-cfb7-4262-9fb7-78f3cb9b2bac)

---

## 🧠 Why This Matters

By simulating real-world ticket flow:

- 🧾 You practice detailed internal documentation
- 🧪 You show Layered troubleshooting logic
- 🔁 You demonstrate professional hand-off techniques

This ensures that **Jin Yang** or any higher-tier tech knows **exactly what’s been tried**, avoiding repetition and saving time.

---

## 🎉 Success!

You’ve now:

- 🛠️ Created a realistic tech support ticket
- 📞 Simulated a client interaction
- 🔎 Documented OSI Layer 1–3 troubleshooting
- 🔁 Reassigned and escalated the ticket professionally
