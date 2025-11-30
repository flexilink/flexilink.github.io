## **FlexiLink: A Deterministic Non-IP Network for Critical Infrastructure**

### **About the Project**

FlexiLink is a next-generation deterministic networking architecture. It is designed as a **non-IP, ultra-low-latency, time‑deterministic backbone** for future communication systems, including:

* Energy networks & smart grid
* Industrial control & automation
* Telecom backbone (5G / 6G)
* Live media, AV, and real-time computing
* Critical national infrastructure

The technology has been put forward to the **ETSI Non‑IP Networking (NIN)** initiative, whose working group is chaired by **John Grant**.

---

## **Key Features**

* **Latency as low as 65μs** for high‑resolution audio
* **Guaranteed delivery** for time‑critical flows
* **Up to 97.6% bandwidth utilisation**
* **Hardware‑proven prototype (Aubergine)**
* **Non‑IP design reduces the attack surface significantly**
* **Compatible with SDN‑style control and slicing**
* **Runs over existing fibre / IP infrastructure when required**

---

## **Project Documentation**

To provide visitors with a clear, structured overview, this section summarises the FlexiLink research and engineering documents already hosted in the GitHub repository. These files are grouped into categories so users can easily understand the scope of work.

### **1. Architecture & Core Design**

Documents explaining FlexiLink’s network model, deterministic routing, and system-level architecture.

* *Eng_Flexilink_Brief02.docx*
* *Flexilink scenarios.pdf*
* *Flexilink for hetnets.pdf*

### **2. Security & Determinism**

Analyses covering security design, minimised attack surface, timing models, and trust boundaries.

* *Flexilink security features v1.pdf*

### **3. Implementation & Hardware Platform**

Engineering details of the FPGA implementation and the Aubergine hardware platform.

* *Aubergine documentation 211009.pdf*
* *Nine Tiles development environment 211010.pdf*
* *Extensions to Flexilink implementation for BCU 231204.pdf*

### **4. Lab Environment & Tutorials**

Materials used for demonstrations, experiments, and academic teaching.

* *Flexilink Lab Tutorial for BCU.pdf*

### **5. Development Tools & Standards Support**

Documents related to protocol processing, virtual machine code, and tooling used in FlexiLink development.

* *TeaLeaves / TeaLogics development documents*

These categories reflect the structure of the current GitHub project files and help visitors navigate the technical landscape effectively.

---

## **Hardware Prototypes**

FlexiLink has been implemented in FPGA as the **Aubergine switch**, featuring:

* Deterministic switching fabric
* Custom soft CPU
* Hardware scheduling
* Real‑time audio/video routing with deterministic latency

---

## **Standards & Collaboration**

FlexiLink contributes to international standardisation:

* **ETSI NIN (Non‑IP Networking)**
* **AES / IEC 62379**
* **Secured time‑critical networking research (Birmingham City University)**

Collaboration enquiries are welcome from regulators, telecom operators, energy companies, and research institutions.

---

## **Additional Resources**

* [Ninetiles](http://www.ninetiles.com/)

## **Publications (from oldest to newest)**

* Wang, Yonghao, John Grant, and Jeremy Foss. *Flexilink: A Unified Low Latency Network Architecture for Multichannel Live Audio*. AES Convention 133, 2012.
* Ma, T., Y. Wang, W. Hu, D. El‑Banna, and K. Zhang. *Evaluation of Flexilink as Unified Real‑Time Protocol for Industrial Networks*. IEEE ICIEA, May 2018.
* Ma, Tianao, Wei Hu, Yonghao Wang, Dalia El‑Banna, John Grant, and Hongjun Dai. *Evaluation of Flexilink as Deterministic Unified Real‑Time Protocol for Industrial Networks*. IEEE TrustCom/BigDataSE, 2018.
* Guo, Yi, Jing Liu, Yonghao Wang, and Wei Hu. *Short Cycle Conversion Scheduling Model for Flexilink Architecture*. IEEE HPCC/SmartCity/DSS, Aug 2019.
* Ma, Rongxuan, Yonghao Wang, Wei Hu, and Mahir Payyanil Karalakath. *Evaluation of Video Payload over Low Latency Networks: Flexilink*. IJ PEDS 35(3), 2020.

---

## **Contact**

For collaboration, demonstrations or briefings:

**Leo Wang – Birmingham City University**
**John Grant – Nine Tiles, Cambridge**
Email: [yonghao.wang@bcu.ac.uk](mailto:yonghao.wang@bcu.ac.uk)
