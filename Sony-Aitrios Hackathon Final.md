# 🧐 SmartChainERP: Our AI-Powered Vision for Smarter Warehousing  
*Sony AITRIOS Hackathon Finalist Blog • Jan 2025 – Ongoing*

## ✨ TL;DR  
We built **SmartChainERP** — an intelligent, real-time warehouse and supply chain system that uses AI, camera sensors, and real-time messaging to optimize inventory management. It's cross-platform, blazing fast, and powered by Sony's IMX-500 camera, MQTT magic, and a full-stack TypeScript + Django setup.

---

## 🌟 Problem Statement  
Modern warehouses are messy. Stockouts, overstocking, and delayed communication between hardware and dashboards are still problems in 2025. Manual errors are common, and traditional ERPs often miss the real-time edge.

So when the **Sony AITRIOS Hackathon** came calling, we asked:

> **What if warehouses could see, think, and act — like living systems?**

---

## 🛠️ Tech Stack Breakdown

| Layer        | Tech Used                                                                 |
|--------------|---------------------------------------------------------------------------|
| 🔍 **Frontend**  | React + TypeScript + Next.js, Tailwind for styling                        |
| 🧠 **Backend**   | Django REST Framework, PostgreSQL, Postman for API testing               |
| ⚙️ **Real-time** | MQTT broker + polling system for live updates                            |
| 👁️ **Hardware**  | Sony IMX-500 camera sensor + Raspberry Pi (for edge detection + control) |
| 🖥️ **Desktop**   | Electron.js for cross-platform deployment                                |

---

## 🧹 Features

### 1. 🔍 **Live Inventory Monitoring**  
Real-time item tracking using the **Sony IMX-500 camera** + **Raspberry Pi**. The camera feeds data to the backend, which is processed instantly and reflected on the dashboard — no delay, no guesswork.

### 2. 📈 **Anomaly Detection**  
If an unexpected item appears (say, a different product or missing one), our system flags it immediately using a lightweight ML model on the edge.

### 3. 🧪 **Test-Driven API Integration**  
We used **Postman** to rigorously test all backend APIs and edge communication. Clean, versioned, and modular endpoints ensured that the hardware, backend, and UI stayed in sync.

### 4. 📡 **MQTT-Based Real-Time Sync**  
We integrated **MQTT** for lightweight messaging between sensors, servers, and the frontend. Combined with polling (as fallback), the system stays updated even in flaky network environments.

### 5. 🖥️ **Cross-Platform Deployment**  
With **Electron**, the entire ERP can run as a desktop app — whether you're on Windows, Mac, or Linux. One codebase to rule all devices.

---

## 🧠 Why It Stood Out in the Hackathon  
This wasn’t just a demo. **SmartChainERP** is a practical, scalable system built with actual hardware integration and production-level architecture. We didn’t stop at a dashboard — we **connected the physical and digital world**, which is exactly what Sony’s AITRIOS platform encourages.

---

## 🏁 Current Status  
- ✅ System architecture and core flows built  
- ✅ Hardware integrated and tested  
- ⚡ Next step: expanding to multi-warehouse support and blockchain audit trail integration (coming soon!)

---

## 🙏 Special Thanks  
Big shoutout to **Sony** for organizing the AITRIOS Hackathon and giving us the opportunity to push boundaries. Also, cheers to the amazing community and mentors who gave early feedback during our build.

---

## 🔗 Wanna Connect?  
Let’s chat about smart warehousing, computer vision, or just why MQTT is criminally underrated. Hit me up on [GitHub](https://github.com/harish-x64) or [LinkedIn](https://linkedin.com/in/harish-x64) 💬
