# 🏗️ Snag Detection & Reporting Platform (AI-Powered)

An advanced, end-to-end snag management system designed for construction sites. This platform leverages **AI Vision (YOLOv8)** to detect building damage (cracks, etc.) from images, generates detailed inspection reports, and facilitates real-time collaboration between Site Engineers and Contractors.

---

## 🚀 Key Features

### 🤖 AI-Powered Detection
- **Vision Agent:** Deep learning model (YOLOv8 via Roboflow API) for automatic damage detection in site photos.
- **Severity Analysis:** Intelligent classification of snags into Low, Medium, and High severity.
- **Automatic Localization:** Merges multiple detections into a single bounding box for precise visualization.
- **Feedback Loop:** Learning agent that evolves based on user feedback.

---

### 👥 Multi-Role Dashboards

#### 👷 Site Engineer
- Project workspace management.
- AI-assisted snag generation from camera/upload.
- Assigning snags to specific contractors.
- Dynamic reporting (Export to PDF and Excel).

#### 🛠️ Contractor
- Real-time task assignments.
- Status tracking (**Pending → In Progress → Resolved**).
- Detailed view of detection results and recommendations.

---

### 📡 Real-time & Automation
- **Socket.IO Integration:** Instant notifications when new snags are assigned or status is updated.
- **Automated Emailing:** Contractors receive detailed AI inspection reports via email with attachments.
- **Offline Support:** Integration with IndexedDB allows capturing snags even without internet.

---

## 🛠️ Technology Stack

### Frontend
- **Framework:** React.js (Vite)
- **Icons:** Lucide React
- **Styling:** Vanilla CSS (Global Design System)
- **Real-time:** Socket.io-client
- **Data Handling:** Axios, XLSX
- **PDF Generation:** jsPDF + jsPDF-AutoTable

---

### Backend
- **Runtime:** Node.js
- **Framework:** Express.js
- **Database:** PostgreSQL
- **Real-time Engine:** Socket.io
- **Authentication:** JWT & Bcryptjs
- **File Handling:** Multer
- **Emailing:** Nodemailer

---

### AI Pipeline (Python)
- **Computer Vision:** OpenCV
- **Deep Learning Interface:** Roboflow API (YOLOv8)
- **Data Processing:** Numpy

---

## 📁 Project Structure
