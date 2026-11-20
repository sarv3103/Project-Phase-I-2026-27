# SecureWheels: Auditable Multimodal Motor Insurance Claim Adjudication & Fraud Detection Platform

**Project Phase-I (2026–27) Submission**  
**Forked From:** `NituPawar/Project-Phase-I-2026-27`  
**Institution:** MGM's College of Engineering, Nanded (Dr. Babasaheb Ambedkar Technological University, Lonere)  
**Department:** Department of Computer Science & Engineering  
**Academic Year:** 2026–2027  

---

## 👥 Student & Project Particulars

* **Candidate Name:** **Sarvesh Sudhir Kulkarni** (Roll No: **102**, Division: **A**) — *Lead Developer & System Architect*
* **Group Members (Co-Authors):**
  - **Chaitanya Rajesh Kopalwar** (Roll No. 101, Computer Vision & Forensics)
  - **Pranav Prashant Kulkarni** (Backend & Machine Learning)
  - **Chandrashekhar Pradip Kalyan** (Frontend & Integration)
* **Project Guide:** **Ms. Linta B. Isal**, Assistant Professor, Dept. of CSE  
* **Project Incharge:** **Ms. Nitu Pawar**, Assistant Professor, Dept. of CSE  

---

## 🌐 Live Production Deployment & Cloud URLs

The platform is deployed and fully operational for evaluation:

* 🚀 **Live Production Application (Vercel):** [**https://securewheels-insurance.vercel.app/**](https://securewheels-insurance.vercel.app/)
* 🗄️ **Cloud Database (Supabase Enterprise):** Managed PostgreSQL 15 with Row-Level Security (RLS) policies.
* ⚡ **Application Server (Render Cloud):** Asynchronous Python 3.11 FastAPI containerized backend.
* 📜 **Government of India Copyright Registration:** Filed under Class *Computer Software* (Diary No: **`SW-54364/2026-CO`**, Receipt No: **`285193`**).

---

## 📁 Submission Checklist & Repository Organization

As per the guidelines for Project Phase-I, this repository contains the complete source code, dataset, database schemas, requirements, and soft copies of all academic documents:

```
Project-Phase-I-2026-27/
├── backend/                       # Complete FastAPI backend, routers, ML fraud detector, services
├── frontend/                      # React 18, TypeScript, Tailwind CSS, Vite web application
├── ml/                            # Machine learning models, training scripts, serialized weights
│   └── data/                      # Vehicle insurance claims benchmark datasets (carclaims.csv)
├── database/                      # Supabase PostgreSQL schemas & migration scripts
├── tests/                         # Comprehensive unit, integration, and security test suites
├── REPORT_AND_DOCUMENTS/          # Complete soft copy of all documents (Print-ready PDF & MD)
│   ├── MAJOR PROJECT REPORT.pdf   # Complete 59-page Major Project Report (Print-Ready)
│   ├── reseaech paper.pdf         # IEEE Conference Research Paper Submission
│   ├── certificate_major.pdf      # College Guide & Department Approval Certificates
│   ├── CHAITANYA _CERTIFICATE.pdf # Co-Author Certificate
│   ├── KALYAN_CERTIFICATE.pdf     # Co-Author Certificate
│   ├── pranav certificate .pdf    # Co-Author Certificate
│   ├── diary.pdf                  # Official B.Tech Project Logbook / Diary
│   ├── GOVERNMENT_COPYRIGHT_OFFICE_OFFICIAL_FEE_RECEIPT_285193.pdf # Official Copyright Fee Receipt
│   ├── GOVERNMENT_COPYRIGHT_STATUS_RECEIPT_SW-54364-2026-CO.pdf    # Copyright Application Status
│   ├── HDFC_BANK_PAYMENT_E_ACKNOWLEDGEMENT_RECEIPT.pdf             # Payment E-Acknowledgement
│   ├── 01_PRIMARY_WORK_SOURCE_CODE_DEPOSIT.pdf                     # Source Code Deposit Document
│   ├── 02_NOC_AND_JOINT_AUTHORSHIP_DECLARATION.pdf                 # Signed Joint Authorship NOC
│   ├── SECUREWHEELS_ACADEMIC_EXHIBITION_POSTER.pdf                 # Project Exhibition Poster
│   └── COLLEGE_VIVA_AND_POSTER_PRESENTATION_SCRIPT.md              # 2-min & 5-min viva script
├── requirements.txt               # Backend Python dependencies
├── .env.example                   # Environment configuration template
├── run.py                         # Local platform launcher
└── README.md                      # Master submission documentation
```

---

## 💡 Key Technological Contributions

1. **Asymmetric Cost-Sensitive Machine Learning Ensemble:**
   - Unites Extreme Gradient Boosting (XGBoost), Random Forest, and Isolation Forest.
   - Embeds a mathematical asymmetric loss matrix ($C_{FN}:C_{FP} = 6:1$) penalizing undetected fraud 6-fold more heavily than surveyor inquiries.
   - Operates at the cost-optimal decision threshold $\theta^* = 0.40$, achieving **89.1% fraud recall**, **82.6% precision**, and saving **34.2% in net carrier underwriting loss**.
2. **Multimodal Computer Vision Forensics Engine:**
   - Enforces 5-angle photographic evidence collection (Front, Rear, Left, Right, Close-up Damage).
   - Dual-layer blur detection using OpenCV discrete Laplacian variance ($\sigma_L^2 < 42.0$).
   - **Senior Forensic Claim Interrogator:** Actively blocks clean showroom-condition vehicles from falsely filing collision claims.
   - **Cross-Perspective Contradiction Engine:** Detects model, generation, and paint color discrepancies across viewpoints.
   - **Error Level Analysis (ELA):** Localizes digital compression tampering and JPEG splicing.
3. **Local & Cloud Operational Flexibility:**
   - The platform runs complete local machine learning inference using bundled Scikit-Learn / XGBoost models, with zero mandatory external API dependencies required for local demonstration.
4. **IRDAI-Compliant Auditable Dossier:**
   - Transparent, human-in-the-loop explainability for insurance adjusters with real-time pipeline re-evaluation.

---

## 🚀 How to Run Locally

### Prerequisites
- Python 3.11+
- Node.js 18+ & npm

### 1. Start the Backend
```bash
python -m venv venv
# On Windows: venv\Scripts\activate | On Linux: source venv/bin/activate
pip install -r requirements.txt
cp .env.example .env
uvicorn backend.main:app --host 0.0.0.0 --port 8000 --reload
```

### 2. Start the Frontend
```bash
cd frontend
npm install
npm run dev
```
Open your browser at `http://localhost:5173`.

---

## 📜 Official Government Copyright Details
* **Work Title:** Insurance Claim Fraud Detection using Ensemble Learning
* **Class of Work:** Computer Software Work
* **Registration Diary No:** `SW-54364/2026-CO`
* **Receipt No:** `285193`
* **Applicant:** Sarvesh Sudhir Kulkarni (Jointly with co-authors)
* **Authority:** Copyright Office, Department for Promotion of Industry and Internal Trade (DPIIT), New Delhi.

---
*Department of Computer Science & Engineering • MGM's College of Engineering, Nanded*
