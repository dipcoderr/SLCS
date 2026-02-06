# 🚦 Street Light Complaint Management System (SLCS)

> **Empowering citizens, streamlining administration.**
> A modern, full-stack solution for smarter civic infrastructure management.

**[🚀 View Live Demo](https://www.google.com/search?q=http://localhost:5173)** · **[🐛 Report Bug](https://www.google.com/search?q=https://github.com/yourusername/repo/issues)** · **[✨ Request Feature](https://www.google.com/search?q=https://github.com/yourusername/repo/issues)**

---

## 🧐 Overview

The **Street Light Complaint Management System** is more than just a reporting tool—it's a digital bridge between the public and municipal authorities.

Built with performance in mind using **Vite** and **Redux**, it allows citizens to securely report malfunctions with **digital signatures** and **visual proof**. Simultaneously, it equips administrators with a powerful dashboard to track, filter, and resolve issues within their specific jurisdictions.

---

## 🌟 Key Features

### 🏛️ For Citizens (User)

* **🔐 Military-Grade Auth:** Secure registration and login powered by **JWT**.
* **📝 Smart Reporting:** Submit complaints with granular details:
* **Location:** Precise area mapping.
* **Evidence:** Image upload support (powered by **Firebase**).
* **Verification:** **Digital signature** support for authenticity.


* **👀 Real-Time Tracking:** Watch your complaint move from `Pending` → `Approved` → `Resolved` instantly.
* **📂 History:** A personal archive of all your reported issues.

### 👮‍♂️ For Authorities (Admin)

* **🛡️ Area-Based Control:** Strict access control ensures admins only manage complaints in their assigned jurisdiction.
* **💬 Remarks System:** Add internal notes, rejection reasons, or resolution details to any ticket.
* **📊 Master Dashboard:** Advanced filtering by **Date**, **Status**, or **Area** to identify high-priority zones.
* **✅ Workflow Management:** One-click approval or denial mechanisms.

---

## 🛠️ The Tech Ecosystem

We chose a high-performance stack to ensure speed, scalability, and developer experience.

### **Frontend (Client)**

| Tech | Badge | Why? |
| --- | --- | --- |
| **React** |  | Component-based UI |
| **Vite** |  | Lightning fast build tool |
| **Redux** |  | Global state management |
| **Tailwind** |  | Modern utility-first styling |

### **Backend (Server)**

| Tech | Badge | Why? |
| --- | --- | --- |
| **Node.js** |  | Scalable runtime |
| **Express** |  | Robust API framework |
| **MongoDB** |  | Flexible NoSQL database |
| **JWT** |  | Stateless authentication |

### **Cloud & Tools**

---

## 📐 System Architecture

The application follows a **Decoupled Monolithic** architecture:

1. **Client:** React (Vite) consumes RESTful APIs.
2. **Server:** Express.js handles business logic, validation, and remarks.
3. **Database:** MongoDB stores users, admins, and complaint documents.
4. **Storage:** Firebase handles heavy media assets (complaint images).

---

## ⚡ Getting Started

### Prerequisites

* Node.js (v14+)
* MongoDB (Local or Atlas)

### 1. Clone & Install

```bash
git clone https://github.com/yourusername/street-light-complaint-system.git
cd street-light-complaint-system

```

### 2. Backend Setup

```bash
cd backend
npm install
# Create .env file with MONGODB_URL and JWT_SECRET
npm start

```

### 3. Frontend Setup

```bash
cd frontend
npm install
# Create .env with VITE_FIREBASE_ config
npm run dev

```

---

## 🛣️ API Roadmap

| Method | Endpoint | Description |
| --- | --- | --- |
| `POST` | `/api/v1/auth/register` | User Registration |
| `POST` | `/api/v1/complaints` | Submit Complaint (w/ Image) |
| `PUT` | `/api/v1/complaints/:id` | **Admin:** Update Status/Remarks |
| `GET` | `/api/v1/users/profile` | **User:** Get Profile & History |

---

## 🤝 Contributing

We welcome contributions!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/NewFeature`)
3. Commit your Changes (`git commit -m 'Add NewFeature'`)
4. Push to the Branch (`git push origin feature/NewFeature`)
5. Open a Pull Request

---

## 👨‍💻 Author

**Dipanshu Kumar Mishra**

* Designed with ❤️ for better cities.

---

### 📄 License

Distributed under the **ISC License**. See `LICENSE` for more information.
