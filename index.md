## **FlexiLink: Secure-by-Design Non-IP Networking for Critical Infrastructure**

### **About the Project**

FlexiLink is a next-generation deterministic networking architecture designed as a **non-IP, ultra-low-latency, time-deterministic backbone** for critical systems, including:

- Energy networks and smart grid
- Industrial control and automation (OT/ICS)
- Telecom backbone (5G/6G evolution)
- Live media and real-time AV workloads
- Wider critical national infrastructure (CNI)

The technology has been proposed to the **ETSI Non-IP Networking (NIN)** initiative.

---

## **What’s New**

- **2026-03-12:** Website refreshed with GitHub organisation links and public repository overview.
- **2026-02-18:** FlexiLink controller source and tooling were released publicly.

---

## **GitHub Organisation**

[![GitHub](https://img.shields.io/badge/GitHub-flexilink-181717?logo=github&logoColor=white)](https://github.com/flexilink)

Explore all public work under the FlexiLink organisation:

- **Organisation home:** [github.com/flexilink](https://github.com/flexilink)

### **Public repositories**

1. **flexilink-controller**  
   FlexiLink controller deliverables and related binary artefacts.  
   Repo: [github.com/flexilink/flexilink-controller](https://github.com/flexilink/flexilink-controller)

2. **flexilink-docs**  
   Research documentation and technical project materials.  
   Repo: [github.com/flexilink/flexilink-docs](https://github.com/flexilink/flexilink-docs)

3. **flexilink.github.io**  
   Public organisation homepage source.  
   Repo: [github.com/flexilink/flexilink.github.io](https://github.com/flexilink/flexilink.github.io)

For controller internals and tooling:

- Controller source directory: [ControllerSRC](https://github.com/flexilink/flexilink-controller/tree/main/ControllerSRC)
- Wireshark plugin for FlexiLink traffic decoding: [WiresharkPlugin](https://github.com/flexilink/flexilink-controller/tree/main/WiresharkPlugin)

---

## **Strategic Positioning**

FlexiLink is positioned as a **clean-slate Non-IP Layer2/3 architecture** aimed at deterministic operation and reduced attack surface in CNI contexts.

Key positioning points:

- **Security-by-design flows:** authenticated flow setup before forwarding data
- **Deterministic behaviour:** engineered for time-critical traffic predictability
- **Legacy migration path:** transparent tunnelling to protect existing Ethernet/IP estates
- **High efficiency:** strong bandwidth utilisation with low per-packet overhead
- **Standardisation direction:** active alignment with ETSI Non-IP networking discussions

---

## **Key Features**

- **Latency as low as 65μs** for high-resolution audio scenarios
- **Guaranteed delivery path** for time-critical wired flows (subject to normal physical-layer assumptions)
- **Up to 97.6% bandwidth utilisation** for user payload in benchmarked scenarios
- **Hardware-proven prototype** (Aubergine FPGA platform)
- **Reduced attack surface** by avoiding always-on IP routing assumptions
- **Compatible migration approach** over existing fibre/IP infrastructure where needed

---

## **Project Documentation**

Initial documentation will continue to expand. Planned content includes:

- Architecture overview
- Core technology and data plane/control plane concepts
- Cloud-based test lab model
- Publications and IP references

---

## **Hardware Prototypes**

FlexiLink has been implemented in FPGA as the **Aubergine switch**, featuring:

- Deterministic switching fabric
- Custom soft CPU approach
- Hardware scheduling
- Real-time audio/video routing with deterministic latency

---

## **Standards & Collaboration**

FlexiLink contributes to international standardisation and collaborative research:

- **ETSI NIN (Non-IP Networking)**
- **AES / IEC 62379 related directions**
- **Security and time-critical networking research (Birmingham City University and partners)**

Collaboration enquiries are welcome from regulators, telecom operators, energy organisations, and research institutions.

---

## **Publications**

1. Wang, Yonghao, John Grant, and Jeremy Foss. *Flexilink: A Unified Low Latency Network Architecture for Multichannel Live Audio*. Audio Engineering Society Convention 133, 2012. [PDF](docs/papers/201210%20Flexilink%20A%20unified%20low%20latency%20network%20architecture%20for%20multichannel%20live%20audio.pdf)

2. Ma, T., Y. Wang, W. Hu, D. El-Banna, and K. Zhang. *Evaluation of Flexilink as Unified Real-Time Protocol for Industrial Networks*. 2018 13th IEEE Conference on Industrial Electronics and Applications (ICIEA), May 2018, 123–28. https://doi.org/10.1109/ICIEA.2018.8397701.

3. Ma, Tianao, Wei Hu, Yonghao Wang, Dalia El-Banna, John Grant, and Hongjun Dai. *Evaluation of Flexilink as Deterministic Unified Real-Time Protocol for Industrial Networks*. 2018 17th IEEE International Conference on Trust, Security and Privacy in Computing and Communications / BigDataSE, 2018, 22–27. [PDF](docs/papers/201808%20TrustCom%20Evaluation%20of%20Flexilink%20as%20Deterministic%20Unified%20Real-Time%20Protocol%20for%20Industrial%20Networks.pdf)

4. Guo, Yi, Jing Liu, Yonghao Wang, and Wei Hu. *Short Cycle Conversion Scheduling Model for Flexilink Architecture*. HPCC/SmartCity/DSS, 2019, 2367–72. https://doi.org/10.1109/HPCC/SmartCity/DSS.2019.00329. [PDF](docs/papers/201908%20Short%20Cycle%20Conversion%20Scheduling%20Model%20forFlexilink%20Architecture.pdf)

5. Ma, Rongxuan, Yonghao Wang, Wei Hu, and Mahir Payyanil Karalakath. *Evaluation of Video Payload over Low Latency Networks: Flexilink*. International Journal of Parallel, Emergent and Distributed Systems 35, no. 3 (2020): 273–87. https://doi.org/10.1080/17445760.2018.1487065. [PDF](docs/papers/201806%20Evaluation%20of%20video%20payload%20over%20low%20latency%20networks%20Flexilink.pdf)

---

## **Contact**

For collaboration, demonstrations, or technical briefings:

- **Dr Yonghao (Leo) Wang** — Birmingham City University  
  Email: `yonghao.wang AT bcu.ac.uk`

- **John Grant** — Nine Tiles, Cambridge  
  Email: `j AT ninetiles.com`

## **Additional Resources**

- [Nine Tiles](http://www.ninetiles.com/)
