# IGS-software 🚀
> **Offline-First Enterprise ERP & GST Billing Software for Retail & Saree/Apparel Stores**

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![Platform](https://img.shields.io/badge/platform-Windows-lightgrey.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Stack](https://img.shields.io/badge/tech--stack-Electron%20%7C%20React%20%7C%20Node.js%20%7C%20SQLite-blueviolet.svg)

**IGS-software** is a fast, reliable, offline-first desktop POS, inventory management, and GST invoicing ERP application built for merchants, apparel/saree showrooms, and retail shop owners. It operates seamlessly without an active internet connection and automatically reconciles store transactions with a central server once online.

---

## ✨ Key Features

- **⚡ Sub-10ms Offline Billing:** Runs directly on local desktop hardware powered by an embedded SQLite engine—no network lag or Internet dependency during customer checkout.
- **🇮🇳 Full GST Engine:** Auto-calculates CGST/SGST for intra-state sales and IGST for inter-state transactions based on merchant and customer state codes.
- **🏷️ Apparel & Saree Dual-Inventory Matrix:**
  - **Single SKUs:** Track unique sarees, silk items, and supplier origins.
  - **Variable SKUs:** Manage size matrices (S, M, L, XL, XXL) linked to parent products.
- **🖨️ Direct ESC/POS Thermal & Label Printing:** Silent USB barcode sticker generation and instant thermal bill printing without print-dialog friction.
- **📈 Sales Commission & Agent Ledger:** Track salesperson sales performance and calculate real-time commission payouts.
- **📊 Customer Retention CRM:** Filter inactive customers (e.g., *"No purchases in 1, 3, or 6 months"*) for targeted marketing.
- **🔄 Outbox Event-Driven Sync:** Queues local sales offline using client-side UUIDs and synchronizes with the cloud once network connectivity is restored.

---

## 🛠️ Tech Stack

- **Desktop Framework:** [Electron](https://www.electronjs.org/)
- **Frontend UI:** [React](https://react.dev/) + [Tailwind CSS](https://tailwindcss.com/) + [Vite](https://vitejs.dev/)
- **Local Database:** [better-sqlite3](https://github.com/WiseLibs/better-sqlite3) (Embedded WAL Mode)
- **Backend Runtime:** Node.js (Main Process)
- **Hardware Drivers:** `node-escpos` / `node-escpos-usb` (Thermal Printing)
- **Installer Build Engine:** `electron-builder` (NSIS Executable output)

---

## 🏗️ System Architecture
