# Fabric Notebooks

A curated collection of **Microsoft Fabric notebooks** focused on Lakehouse management, Delta table governance, and safe, repeatable data engineering patterns.

This repository is intended for:
- Data Engineers
- Analytics Engineers
- BI / Platform Engineers
- Teams working in **Microsoft Fabric** and **Delta Lake**

---

## 📓 DeltaPropEnforcer.ipynb

### Purpose
**DeltaPropEnforcer** is a production‑ready Fabric notebook that safely enforces Delta table properties across a Lakehouse.

It is designed to help teams:
- Standardize Delta table configurations
- Prevent configuration drift
- Apply properties in a controlled, auditable way

### Key Features
- ✅ **Dry‑run mode** (preview changes before applying)
- 🔁 **Idempotent execution** (safe to re‑run)
- 🛡 **Guardrails** to avoid overwriting existing intentional settings
- 📊 Clear logging of applied vs skipped properties
- ⚙️ Works at **scale** across multiple tables

### Example Use Cases
- Enforcing auto‑optimize / auto‑compaction standards
- Applying consistent retention or checkpoint policies
- Aligning table properties across dev / test / prod Lakehouses
- Supporting governance and operational readiness in Fabric

---

## 🚀 How to Use in Microsoft Fabric

1. Open **Microsoft Fabric**
2. Navigate to your **Workspace**
3. Create or open a **Notebook**
4. Use **Import notebook** and upload `DeltaPropEnforcer.ipynb`
5. Attach the notebook to your target **Lakehouse**
6. Run in **dry‑run mode first** to validate changes
7. Disable dry‑run to apply properties

> ⚠️ Always validate against non‑production Lakehouses first.

---

## 🧱 Design Philosophy

This notebook follows real‑world data platform principles:
- Explicit > implicit behavior
- Safe defaults
- Repeatability over one‑off scripts
- Clear visibility into system‑level changes

It is intentionally written to be **readable, auditable, and extensible** by other engineers.

---

## 🔧 Tech Stack
- Microsoft Fabric
- Fabric Notebooks
- Delta Lake
- Lakehouse architecture

---

## 📂 Repository Structure
```
.
├── DeltaPropEnforcer.ipynb
├── README.md
└── LICENSE
```

---

## 👤 Author
**Mason Piwonka**  
Business Intelligence Analyst & Data Professional  
Specializing in healthcare analytics, Microsoft Fabric, and scalable data platforms

---

## 📄 License
This project is licensed under the terms of the **MIT License**.

