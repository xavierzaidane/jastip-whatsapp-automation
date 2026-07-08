# AI WhatsApp Jastip Automation (n8n + AI Vision + Supabase)

An end-to-end WhatsApp automation workflow that handles customer inquiries, product screenshots, shipping quotations, payment verification, and order management — powered by AI.

**Customer sends a message → AI understands the request → Calculates shipping costs → Creates an order → Admin gets notified automatically.**

No coding required after setup. Built entirely with **n8n**, **WhatsApp**, **Gemini AI**, **Supabase**, and external shipping APIs.

![n8n](https://img.shields.io/badge/n8n-workflow-ff6d5a)
![AI](https://img.shields.io/badge/AI-Gemini-blue)
![license](https://img.shields.io/badge/license-MIT-green)

---

# Features

**AI-powered customer service**
**AI Vision for product screenshots**
**Automatic shipping quotation**
**RMB → IDR conversion**
**Shipping cost calculation**
**Payment receipt verification**
**WhatsApp admin notifications**
**Supabase order management**
**Conversation memory**

---

# Workflow Overview
<p align="center">
  <img src="docs/workflow.png" alt="Workflow" width="100%">
</p>

---

# What's Inside

| Workflow | Description |
|-----------|-------------|
| **WhatsApp Trigger** | Receives incoming customer messages |
| **AI Vision Classifier** | Detects product screenshots, payment receipts, or unrelated images |
| **AI Customer Assistant** | Collects missing information and guides customers through the ordering process |
| **Exchange Rate Service** | Retrieves the latest RMB to IDR exchange rate |
| **Shipping Calculator** | Calculates domestic shipping costs based on destination |
| **Invoice Generator** | Calculates total payment automatically |
| **Supabase Integration** | Stores customer orders and conversation data |
| **Admin Notification** | Sends payment confirmations and important events to WhatsApp groups |

---

# Supported Customer Flow

### Product Inquiry

Customer sends:

- Product screenshot
- Product link
- Product information

↓

AI extracts:

- Product name
- Price (RMB)

↓

AI asks for:

- Destination
- Shipping method
- Estimated weight

↓

Shipping cost is calculated automatically.

---

### Shipping Quotation

Customer provides:

- Destination
- Shipping method
- Weight
- Product price

↓

Workflow calculates:

- Product cost
- Shipping cost
- Service fee
- Total invoice

---

### Payment Verification

Customer uploads payment receipt.

↓

AI Vision classifies the image.

↓

Receipt is forwarded to the admin.

↓

Order status is updated automatically.

---

# Tech Stack

- n8n
- Gemini AI
- WhatsApp (WAHA API)
- Supabase
- Google Gemini Vision
- Biteship API
- Exchange Rate API

---

# Setup (~10 Minutes)

1. Import the workflow into n8n.
2. Configure your credentials:
   - WhatsApp API
   - Gemini API
   - Supabase
   - Shipping API
   - Exchange Rate API
3. Update your environment variables.
4. Configure your Supabase tables.
5. Activate the workflow.
6. Connect your WhatsApp number.
7. Start receiving customer messages.

---

# AI Capabilities

The assistant can:

- Understand natural language
- Read product screenshots
- Extract RMB prices
- Answer customer questions
- Calculate quotations
- Maintain conversation memory
- Detect payment receipts
- Escalate orders to admins

---

# Use Cases

- Personal Shopper (Jastip)
- Import & Forwarding Services
- WhatsApp AI Customer Service
- Cross-border E-commerce
- Small Business Automation

---


