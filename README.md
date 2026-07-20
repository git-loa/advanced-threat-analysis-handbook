
# **Advanced Threat Analysis and Detection Engineering Handbook**

This handbook is a comprehensive, long-term reference for analysts working across Cyber Threat Intelligence (CTI), threat hunting, detection engineering, and SIEM operations. It is designed to support real-world investigations using Splunk (SPL), Microsoft Sentinel (KQL), and Linux endpoint telemetry. The content is structured to reflect the workflows, techniques, and analytical approaches used by modern security teams.

The handbook emphasizes practical, operational knowledge rather than abstract theory. Every section includes detailed explanations, behavioral context, and platform-specific examples that can be applied directly in enterprise environments. Whether you are building detections, performing hunts, analyzing adversary behavior, or designing dashboards, this handbook provides a structured foundation for advancing your skills.

---

## **Purpose**

The goal of this handbook is to unify CTI, threat hunting, detection engineering, and SIEM analysis into a single, cohesive reference. It is written to help analysts:

- Understand adversary behaviors and translate them into operational detections  
- Build high-fidelity SPL and KQL queries  
- Develop repeatable hunting and detection playbooks  
- Investigate Windows and Linux systems effectively  
- Create dashboards that support real-time monitoring  
- Apply CTI workflows to guide hunts and detections  
- Develop advanced detection patterns that remain resilient over time  

---

## **Structure**

The handbook is organized into modular sections, each focusing on a core area of modern security operations:

1. **Introduction**  
2. **Splunk and SPL Fundamentals**  
3. **Windows Investigations**  
4. **Linux Investigations**  
5. **Threat Hunting Fundamentals**  
6. **Detection Engineering Fundamentals**  
7. **Dashboard Design**  
8. **CTI Workflows**  
9. **Threat Hunting Playbooks**  
10. **Detection Playbooks**  
11. **Advanced Detection Patterns**  

Each section is stored as a standalone LaTeX file under `sections/` and imported through `main.tex`.

---

## **Technologies Covered**

- **Splunk (SPL)**  
- **Microsoft Sentinel (KQL)**  
- **Windows Endpoint Analysis**  
- **Linux Endpoint Analysis**  
- **CTI Integration**  
- **Behavioral Detection Concepts**  
- **Threat Hunting Workflows**  

---

## **Intended Audience**

This handbook is designed for:

- CTI Analysts  
- Threat Hunters  
- Detection Engineers  
- SOC Analysts  
- Blue Teamers  
- Security Researchers  
- Students and professionals seeking to advance their defensive skills  

It is also suitable as a portfolio artifact for demonstrating technical depth and operational understanding.

---

## **Usage**

The handbook can be used as:

- A **reference guide** during investigations  
- A **training resource** for new analysts  
- A **portfolio piece** for job applications  
- A **knowledge base** for building detections and hunts  
- A **framework** for designing dashboards and workflows  

Each section is self-contained, allowing readers to jump directly to the topic they need.

---

## **Build Instructions**

This handbook is written in LaTeX and can be built locally or automatically using GitHub Actions. PDF files are **not** committed to the repository; they are generated during CI.

### **Local Build (Optional)**

Install a LaTeX distribution such as TeX Live or MiKTeX, then run:

```
pdflatex main.tex
```

Running twice is recommended to ensure the table of contents and references resolve correctly.

---

### **GitHub Actions Build (Recommended)**

The repository includes a workflow that automatically:

- installs TeX Live  
- compiles `main.tex`  
- generates `main.pdf`  
- uploads the PDF as an artifact  

To download the latest PDF:

1. Open the **Actions** tab  
2. Select the latest workflow run  
3. Scroll to **Artifacts**  
4. Download `handbook-pdf`  

This contains the compiled `main.pdf`.

---

## **Repository Structure**

```
advanced-threat-analysis-handbook/
│
├── main.tex
├── README.md
├── LICENSE
├── .gitignore
│
├── sections/
│   ├── 001_introduction.tex
│   ├── 002_spl_fundamentals.tex
│   ├── 003_windows_investigations.tex
│   ├── 004_linux_investigations.tex
│   ├── 005_threat_hunting_fundamentals.tex
│   ├── 006_detection_engineering_fundamentals.tex
│   ├── 007_dashboard_design.tex
│   ├── 008_cti_workflows.tex
│   ├── 009_threat_hunting_playbooks.tex
│   ├── 010_detection_playbooks.tex
│   └── 011_advanced_detection_patterns.tex
│
└── .github/workflows/
    └── build-pdf.yml
```

---

## **License**

This handbook is intended for educational and professional development purposes.  
You may adapt or extend it for your own learning or internal organizational use.

---

## **Author**

Created by **Leonard**, Toronto-based analyst specializing in:

- Cyber Threat Intelligence  
- Threat Hunting  
- Detection Engineering  
- SIEM Operations  
- Endpoint Analysis  
- Post‑Quantum Cryptography Research  
