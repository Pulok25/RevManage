# RevManage — Subscription & Billing Management System

> **Specialized Billing Engine for DocSheba**  
> Built with MERN Stack (MongoDB, Express, React, Node.js), Tailwind CSS, and **GSAP (GreenSock) Animations**.

---

## 🎨 Design System & Color Tokens

| Token | Light Mode | Dark Mode | Semantic Role |
|---|---|---|---|
| **Primary Brand** | `#4F46E5` | `#6366F1` | Main functional CTAs, active highlights |
| **Neutral Deep** | `#1E293B` | `#E2E8F0` | Dense ledger typography & structural headers |
| **Background (App)** | `#F1F5F9` | `#0B0F19` | Soft, anti-glare canvas background |
| **Surface (Cards/Rows)** | `#FFFFFF` | `#1E293B` | Clean spreadsheet and grid rows |
| **Text (Primary)** | `#0F172A` | `#F1F5F9` | Primary transactional ledger items |
| **Text (Secondary)** | `#475569` | `#94A3B8` | Tax brackets, SKU numbers, timestamps |
| **Status: Settled** | `#0D9488` | `#2DD4BF` | Balanced books, successful renewals |
| **Status: Action Req.** | `#EA580C` | `#FB923C` | Upcoming payment due, dunning retry |
| **Status: Error/Void** | `#E11D48` | `#FB7185` | Voided or disputed bills |

---

## 🎬 GSAP Animation Integration

The application uses **GSAP (`gsap`, `@gsap/react`)** for:
- **Numerical Counters**: Real-time counter interpolation (`animateCounter`) on MRR, ARR, Active Subscribers, and Recovery rate cards.
- **Staggered Entry**: Cascading entry animations (`animateStaggerIn`) on financial grid cards, pricing tiers, and spreadsheet ledger rows.
- **Micro-interactions**: Interactive pulse feedback (`pulseElement`) on retry actions and renewal triggers.
- **Tab Transitions**: Smooth view fades and slide transitions between dashboard modules.

---

## 📋 Features & PRD Workflow Coverage

### 1. User & Admin Account Management
- Multi-persona simulation: **DocSheba Subscribers**, **Clinic Owners**, **Health Care Facility Managers**, and **Hospital Administrators**.
- Multifactor Authentication (MFA) toggle with verification status.
- Role-based user control (RBAC) with granular permissions display.

### 2. Automated Renewal & Payment Gateway Integration (Workflows W-2 & W-3)
- Tiered catalog: Solo Practitioner ($29), Clinic Standard ($89), Facility Pro ($199), Hospital Enterprise ($499).
- Billing interval selector (Monthly vs Annual with 20% discount).
- Simulated Payment Gateways: Stripe (Card/Apple Pay) and SSLCOMMERZ / bKash.
- Interactive **Renewal Simulator** supporting both normal automated renewal and payment failure / dunning trigger.

### 3. Transaction Management (Feature 4)
- Audit-ready spreadsheet ledger with status badges (Settled, Action Required, Error/Void).
- Real-time search and filter tabs.
- One-click "Retry & Settle" with real-time balance balancing.
- Detailed modal invoice receipts.

### 4. Dunning Management (Feature 5)
- Automated grace period tracker (7 calendar days).
- Multi-stage notification dispatch (Email, SMS, in-app alerts).
- Soft retries and grace window expiration tracking.

---

## 🚀 Getting Started

### 1. Install Dependencies
```bash
# Backend
cd backend
npm install

# Frontend
cd ../frontend
npm install
```

### 2. Run the Development Servers
From the root workspace:

```bash
# Run Backend (Port 5000)
npm run dev:backend

# Run Frontend (Port 5173 with API Proxy to 5000)
npm run dev:frontend
```

Alternatively:
- Backend: `cd backend && npm run dev`
- Frontend: `cd frontend && npm run dev`

Open your browser at `http://localhost:5173`.
# RevManage
