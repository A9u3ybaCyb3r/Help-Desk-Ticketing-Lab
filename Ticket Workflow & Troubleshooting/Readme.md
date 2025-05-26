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
3. Sign in with a non-admin user (like Jared):

   * **Email:** `jared@jared.com`
   * **Password:** `jared`

---

## 🆕 Step 1: Create a New Ticket

1. On the left sidebar, click **Create Ticket ➕**
2. Fill out the form:

| Field       | Value                                                      |
| ----------- | ---------------------------------------------------------- |
| Title       | Need Help Installing Outlook                               |
| Description | Hello Help Desk, could you please help me install Outlook? |
| Client      | Monica                                                     |
| Engineer    | Jared (yourself)                                           |
| Type        | Feature Request                                            |

3. Click **Create Ticket ✅**
4. Navigate to **Jared's Open Tickets** to view it.

---

## 💬 Step 2: Add Comments to a Ticket

1. Click on the ticket.
2. Scroll to the **Comments** section.
3. Add a comment like:

```
Remoted into Monica’s PC and installed Outlook. Closing ticket.
```

4. Mark as **Public** or leave **Internal**
5. Click **Comment ➤**
6. Click **Close Issue ⏑**

✅ This moves the ticket to **Closed Tickets**.

---

## 🌐 Step 3: Create Another Ticket with Escalation

1. Go to **Create Ticket ➕**
2. Example:

| Field       | Value                      |
| ----------- | -------------------------- |
| Title       | Network Connectivity Issue |
| Description | Users reporting outage     |
| Client      | Gavin                      |
| Engineer    | Jared                      |
| Type        | Incident                   |

3. Click **Create Ticket**

---

## ♻️ Step 4: Escalate & Reassign the Ticket

1. Go to **Jared’s Open Tickets** and open the network ticket.
2. Add an internal comment:

```
Received call from Gavin reporting a network outage. Escalating to Network Engineer.
```

3. Click **Comment ➤**
4. Click the **Reassign** icon and assign to **Jin Yang**

---

## 🚦 Step 5: Update Ticket Priority & Status

As **Jin Yang**:

* Login: `jinyang@jinyang.com` | Password: `jinyang`
* Go to **Open Tickets** and open the reassigned one

### 📃 Update Priority:

* Click the **priority** label (e.g., Normal)
* Set to **High**

### 🏷️ Update Status:

* Change from **Need Support** → **In Progress**
* Then, change to **Done**

---

## ✅ Step 6: Resolve and Close the Ticket

As **Jin Yang**:

1. Add comment:

```
Resolved issue: unplugged router was reconnected. Connectivity restored.
```

2. Click **Comment ➤**
3. Click **Close Issue**

---

## 🧠 Key Takeaways

* 👤 Help desk users manage tickets
* ♻️ Tickets are reassignable
* 📜 Comments improve clarity
* 🟢 Priority & tags help triage
* 🧼 Always close with notes

---

# ⚠️ Peppermint Ticket Interrupt Lab: Layered Troubleshooting & Escalation

Simulate a **realistic escalation** by documenting a support call to Layer 3:

* 📈 Create a ticket
* 🔍 Ask diagnostic questions
* 🤝 Document all steps
* 🚀 Escalate to another tech

---

## 🔧 Scenario Summary

> Monica calls: “My internet won’t work!”

### Action Plan:

1. Create ticket for Monica
2. Add detailed troubleshooting notes
3. Document Layer 1–3 OSI diagnostics
4. Escalate to another tech (e.g., Jin Yang)

---

### 🔍 Diagnostic Questions

Ask in the comment:

* What do you see in the browser?
* Error messages?
* Are other devices affected?
* Have you rebooted the router?
* Are indicator lights active?

---

### 🔧 Layer 1–3 Troubleshooting

#### Layer 1 – Physical

* Check Ethernet cable
* Confirm link light

#### Layer 2 – Data Link

* Data light flashing?

#### Layer 3 – Network

* Run `ipconfig`
* Do they have a valid IP?
* 169.x.x.x = DHCP issue?
* Confirm DNS and gateway

---

### 📋 Internal Comment Example

> Walked customer through Layer 1–3. Cable good. Link and data lights on. IP = 169.x.x.x. No web access. Escalating.

---

### ♻️ Reassign the Ticket

* Assign to **Jin Yang**
* Set **Priority** to `High`
* Update status if needed

---

## 🧠 Why This Matters

You demonstrate:

* Clear documentation
* Technical thinking
* Support professionalism
* Efficient escalation

---

## 🎉 Success!

You now:

* 🔧 Created a real-world help desk ticket
* 📞 Simulated a user interaction
* 🔎 Documented OSI Layer troubleshooting
* ♻️ Escalated appropriately

This is the level of quality expected in real IT, SOC, or analyst roles. 💼💡
