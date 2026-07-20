# **Advanced Threat Analysis and Detection Engineering Handbook**

This handbook is a comprehensive, long-term reference for analysts working across Cyber Threat Intelligence (CTI), threat hunting, detection engineering, and SIEM operations. It is designed to support real-world investigations using Splunk (SPL), Microsoft Sentinel (KQL), and Linux endpoint telemetry. The content is structured to reflect the workflows, techniques, and analytical approaches used by modern security teams.

The handbook emphasizes practical, operational knowledge rather than abstract theory. Every section includes detailed explanations, behavioral context, and platform-specific examples that can be applied directly in enterprise environments. Whether you are building detections, performing hunts, analyzing adversary behavior, or designing dashboards, this handbook provides a structured foundation for advancing your skills.

---

## **Purpose**

The goal of this handbook is to unify CTI, threat hunting, detection engineering, and SIEM analysis into a single, cohesive reference. It is written to help analysts:

- Understand adversary behaviors and translate them into operational detections  
- Build high-fidelity SPL and KQL queries  
- Develop repeatable hunting and detection playbooks  
- Investigate Linux systems effectively  
- Create dashboards that support real-time monitoring  
- Apply CTI workflows to guide hunts and detections  
- Develop advanced detection patterns that remain resilient over time  

---

## **Structure**

The handbook is organized into modular sections, each focusing on a core area of modern security operations:

1. **Introduction**  
2. **Splunk and SPL Fundamentals**  
3. **Threat Hunting Fundamentals**  
4. **Detection Engineering Fundamentals**  
5. **Dashboard Creation**  
6. **Linux Investigation Commands**  
7. **CTI Workflows**  
8. **Threat Hunting Playbooks**  
9. **Detection Playbooks**  
10. **Advanced Detection Patterns**  

Each section is stored as a standalone LaTeX file under `parts/` and imported through `main.tex`.

---

## **Technologies Covered**

- **Splunk (SPL)**  
- **Microsoft Sentinel (KQL)**  
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
├── parts/
│   ├── introduction.tex
│   ├── spl_fundamentals.tex
│   ├── threat_hunting_fundamentals.tex
│   ├── detection_engineering_fundamentals.tex
│   ├── dashboard_design.tex
│   ├── linux_investigations.tex
│   ├── cti_workflows.tex
│   ├── threat_hunting_playbooks.tex
│   ├── detection_playbooks.tex
│   └── advanced_detection_patterns.tex
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

- **Cyber Threat Intelligence**  
- **Threat Hunting**  
- **Detection Engineering**  
- **SIEM Operations**  
- **Endpoint Analysis**  
- **Post‑Quantum Cryptography Research**  
