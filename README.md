# 🛡️ AtHash Guardian: POPIA-Compliant Security Command Center

**The Zaziza Holdings security nucleus.** A zero-trust, real-time compliance dashboard for monitoring and enforcing data governance across South African enterprises.

---

## 🎯 Overview

AtHash Guardian is a **next-generation identity and compliance security platform** built for enterprises operating under **POPIA** (Protection of Personal Information Act) and other jurisdictional data protection frameworks. It provides:

- **Real-time threat monitoring** with AI-driven risk detection
- **PII redaction & anonymization** at scale
- **Zero-trust pipeline orchestration** (data flow validation & encryption)
- **Immutable audit ledger** (blockchain-backed transaction logs)
- **B-BBEE compliance tracking** (South African economic transformation)
- **Multi-node topology visualization** with live data flow monitoring

---

## ✨ Key Features

### 🔐 Guardian Command Center
- **Live threat assessment** — Real-time risk scoring and vulnerability alerts
- **Status monitoring** — Zero-trust enforcement indicators and node health
- **PII counter** — Tracks masked/redacted sensitive data (SA ID numbers, etc.)
- **AI Sentinel** — Automated threat detection across data flows

### 🔄 Zero-Trust Pipeline Orchestration
- **Active pipeline management** — Create, monitor, and validate data flows
- **State machine enforcement** — Each pipeline locked in approved states
- **Guardian actions** — Automated PII masking, encryption verification, compliance checks
- **Real-time sync status** — Healthy / Running / Degraded state indicators

### 🇿🇦 POPIA & Compliance Monitoring
- **Data residency enforcement** — Ensure data remains within AWS Cape Town region
- **Demographic reporting** — B-BBEE auto-reporting via DeltaPro integration
- **Compliance badges** — Visual indicators for LEVEL 1 READY status
- **South African governance** — Tailored for local regulatory requirements

### 📋 Immutable Audit Ledger
- **Blockchain-backed transaction log** — Cryptographic proof of all system actions
- **Tamper-proof records** — Block hashes, timestamps, action descriptions
- **Compliance evidence** — Ready for regulatory audits and legal proceedings
- **Full reconstruction** — Replay audit chain to prove data integrity

---

## 🛠 Technology Stack

| Layer | Technology |
|-------|------------|
| **Frontend** | HTML5 + Tailwind CSS + Phosphor Icons |
| **Canvas Rendering** | Web Canvas API (topology visualization) |
| **State Management** | Vanilla JavaScript (App object pattern) |
| **Authentication** | Biometric fingerprint verification (demo) |
| **Data Format** | JSON + encrypted payloads |
| **Styling** | Dark mode glassmorphic UI |

---

## 🚀 Quick Start

### 1. **Deploy Locally**
```bash
git clone https://github.com/SPVNgcobo/AtHash-Inc.
cd AtHash-Inc
# Open in browser
open index.html
# or
python3 -m http.server 8000
```

### 2. **Access the System**
- **URL**: `http://localhost:8000`
- **Login**: Click "Verify Identity" (demo mode bypasses MFA)
- **Username**: Admin (demo)
- **System Status**: Automatically shows "ONLINE"

### 3. **Navigate Key Sections**
| Section | Purpose |
|---------|---------|
| **Command Center** | Dashboard with KPIs and topology |
| **Zero-Trust Pipelines** | Manage active data flows |
| **POPIA Monitor** | Compliance status tracking |
| **Immutable Ledger** | Audit trail and transaction history |

---

## 📊 Core Workflows

### Threat Scanning Workflow
1. Click **"Run Threat Scan"** in the header
2. Real-time scanning animation activates (2.5s)
3. Threat level updates to **"Secure"** (green check)
4. Event logged to **Immutable Ledger**
5. Toast notification confirms: *"Scan Complete: Zero Threats Found"*

### Pipeline Creation Workflow
1. Go to **Zero-Trust Pipelines** tab
2. Click **"New Pipeline"** button
3. Auto-generated pipeline: `Data_Sync_v2`
4. Status: **RUNNING** → Initializing Guardian
5. Pipeline added to active table with state machine enforcement

### Audit Log Inspection
1. Navigate to **Immutable Ledger** tab
2. View real-time transaction records
3. Each record includes:
   - Block hash (truncated 0x format)
   - Timestamp (UTC)
   - Action description
4. Scroll to see full audit history

---

## 🔒 Security Principles

### Zero-Trust Architecture
- Every data flow validated against policy
- Encryption verified before transmission
- PII automatically redacted at ingestion
- No implicit trust, all actions logged

### POPIA Compliance
- Automated SA ID masking (prevents leakage)
- Data residency enforcement (Cape Town region)
- Consent tracking (audit trail proves opt-in)
- Right-to-erasure support (marked for deletion)

### Immutable Records
- Blockchain-style hash chaining
- Tamper detection via hash mismatch
- Full replay capability
- Legal admissibility for disputes

---

## 📁 Project Structure

```
AtHash-Inc./
├── index.html           # Single-page app (all UI)
├── logo.png            # Zaziza Guardian branding
├── README.md           # This file
└── [No dependencies]   # Zero external libraries (CDN only)
```

---

## 🧩 UI Components

### Main Sections
- **Sidebar Navigation** — Guardian modules (Command Center, Orchestration, Compliance, Audit)
- **Header** — Page title + Threat Scan trigger
- **Main Content** — Tab-based views (Overview, Orchestration, Compliance, Audit)
- **Toast Layer** — Notifications (bottom-right stack)

### Visual Indicators
- **Status Dots** — Green = Active, Red = Error, Yellow = Warning
- **Border Colors** — Gold (#3B82F6) accents for interactive elements
- **Scanning Line** — Animated scan effect during threat analysis
- **Badges** — Status pills (COMPLIANT, LEVEL 1 READY, RUNNING, etc.)

---

## 🎬 Demo Walkthrough

### Scenario: Compliance Audit
1. **Login** → Click fingerprint button
2. **Dashboard** → Review Guardian Status (Active)
3. **Run Scan** → Monitor threat detection
4. **Pipelines** → Inspect data flows (HR_Onboarding_Bot, Finance_Recon_ZA)
5. **Compliance** → Verify POPIA & B-BBEE status
6. **Audit** → Download proof for auditors

### Expected Outputs
- ✅ Guardian Status: **ACTIVE**
- ✅ PII Redacted: **1,204+ SA ID numbers**
- ✅ Threat Level: **SECURE**
- ✅ Pipelines: **3 active**, all healthy
- ✅ Compliance: **COMPLIANT + LEVEL 1 READY**

---

## 🔧 Configuration

### Theme Customization (Tailwind Config)
```javascript
colors: {
  background: '#030712',
  surface: '#0B1120',
  primary: '#3B82F6',      // Primary blue
  secondary: '#10B981',    // Success green
  warning: '#F59E0B',      // Warning amber
  danger: '#EF4444'        // Error red
}
```

### API Integration Points (Future)
- `/api/pipelines` — Fetch active data flows
- `/api/compliance` — Pull real POPIA compliance data
- `/api/audit` — Stream audit logs from backend
- `/api/scan` — Trigger actual threat scanning

---

## 📋 Known Limitations

- **Demo Mode** — No persistent database (refresh resets state)
- **Static Data** — Pipelines hardcoded for demonstration
- **Mock Biometric** — Fingerprint verification simulated
- **Local Storage Only** — No backend integration yet
- **Single-User** — No multi-tenant support

---

## 🚀 Future Roadmap

- [ ] Backend integration (REST API)
- [ ] Real biometric authentication
- [ ] Live threat feeds (OSINT integration)
- [ ] Multi-node cluster support
- [ ] Elasticsearch audit storage
- [ ] Machine learning threat models
- [ ] Mobile app (native compliance)
- [ ] SIEM platform integration

---

## 🤝 Contributing

To extend AtHash Guardian:

1. **Add new pipeline types** in `App.Orchestration.data`
2. **Extend audit actions** via `App.Audit.log()`
3. **New compliance checks** in `/page-compliance` tab
4. **Custom threat models** in `App.UI.triggerScan()`

---

## 📄 License

**MIT License** — Built by S.P. Ngcobo for Zaziza Holdings

---

## 💬 Support & Contact

- **Issues**: [GitHub Issues](https://github.com/SPVNgcobo/AtHash-Inc./issues)
- **Documentation**: [Zaziza Security Hub](https://docs.zaziza-technologies.com)
- **Email**: security@zaziza-technologies.com

---

**Version**: 1.0.0  
**Status**: Production Ready (Demo)  
**Last Updated**: June 2026  
**Target Market**: South African enterprises (POPIA-regulated)
