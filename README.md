# GESTHOS

**GESTHOS** (Gestión de Equipos y Servicios Técnicos Hospitalarios) is an open-source web platform for managing biomedical equipment maintenance in Peruvian public hospitals. It digitizes the complete workflow of maintenance orders, technical specifications, and historical logs, following MINSA's official formats.

<p align="center">
  <img src="https://user-images.githubusercontent.com/your-demo-banner.png" alt="GESTHOS Banner" width="80%"/>
</p>

## 🔧 Features

- ✅ User Management (Admin / Health / Technician)
- ✅ Biomedical Inventory Visualization
- ✅ OTM (Orden de Trabajo de Mantenimiento) Digital Workflow
- ✅ Technical Sheet (FT) Registration *(partially planned)*
- ✅ Historical Log (RH) Automation *(partially planned)*
- ✅ Equipment QR Identification via camera or uploaded image
- ✅ Secure Login with Token Authentication
- ✅ Real-time status updates and PDF export

---

## 📂 Project Structure

| Repository | Description |
|-----------|-------------|
| [bio-data-nextjs](https://github.com/storres20/bio-data-nextjs) | Frontend (Next.js 14 App Router + Tailwind CSS) |
| [bio-data](https://github.com/storres20/bio-data) | Backend (Node.js + Express + MongoDB + JWT + WebSockets) |

---

## 🖥️ Frontend Setup

```bash
git clone https://github.com/storres20/bio-data-nextjs
cd bio-data-nextjs
pnpm install
pnpm dev
```

Configure environment variables:

```env
NEXT_PUBLIC_API_URL=http://localhost:3001
```

---

## 🚀 Backend Setup

```bash
git clone https://github.com/storres20/bio-data
cd bio-data
npm install
npm start
```

Create a `.env` file:

```env
PORT=3001
MONGO_URI=your_mongodb_connection
JWT_SECRET=your_secret_key
```

---

## 📱 QR Scanner Example

Users can scan QR codes attached to equipment using their webcam or upload images. This retrieves full device metadata and links to maintenance records instantly.

<p align="center">
  <img src="https://user-images.githubusercontent.com/your-demo-scanner.png" alt="QR Scanner" width="70%"/>
</p>

---

## 📑 Sample OTM Digital Form

<p align="center">
  <img src="https://user-images.githubusercontent.com/your-demo-otm.png" alt="OTM Digital" width="80%"/>
</p>

---

## 📤 Export to PDF

Users can export official MINSA-compatible formats of:

- OTM
- FT *(planned)*
- RH *(planned)*

---

## 📌 Tech Stack

- **Frontend**: Next.js 14 (App Router), Tailwind CSS, WebSockets
- **Backend**: Node.js, Express.js, MongoDB, JWT, WebSocket
- **Database**: MongoDB (Mongoose)
- **QR Scanning**: `html5-qrcode` for camera and image support
- **PDF Export**: `html2canvas`, `jsPDF` *(frontend)* and `reportlab` *(planned in Python backend)*

---

## 🏥 Real Context of Use

GESTHOS was designed based on real workflows in Peruvian public hospitals. It mirrors the current paper-based processes used by hospital maintenance teams, especially:

- Biomedical engineers
- Health technology managers
- Maintenance technicians

---

## 📃 License

MIT License. See `LICENSE` file for details.

---

## 🙌 Acknowledgments

GESTHOS was created by [Italo Lon Kan Pérez](https://github.com/storres20), Electronic Engineer and Health Technology Manager. The project is part of national efforts to improve traceability and digitalization in healthcare services.

---

## 📬 Contact

If you’re interested in deploying GESTHOS in your hospital or contributing to its development:

📧 italo.lonkan.p@gmail.com  
🌐 [LinkedIn](https://www.linkedin.com/in/italo-lon-kan/)  
