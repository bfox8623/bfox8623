<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:1f6feb&height=130&section=header&text=bfox8623&fontColor=e6edf3&fontSize=42&fontAlignY=40&desc=Universitas%20Jember%20%C2%B7%20Faculty%20of%20Mathematics%20and%20Natural%20Sciences&descSize=14&descAlignY=65&descColor=8b949e" alt="header" width="100%" />

<a href="https://github.com/bfox8623">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&pause=1800&color=58A6FF&center=true&vCenter=true&width=640&lines=Physics+Student;Computational+Physics+%7C+Nuclear+Research;Robotics+%26+Embedded+Systems" alt="Typing SVG" />
</a>

<br/>

![Profile views](https://komarev.com/ghpvc/?username=bfox8623&label=profile%20views&color=1f6feb&style=flat-square)
![OpenMC](https://img.shields.io/badge/OpenMC-0.15.3-1f2937?style=flat-square)
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white)
![Arch Linux](https://img.shields.io/badge/Arch_Linux-1793D1?style=flat-square&logo=archlinux&logoColor=white)

<br/>

[![About](https://img.shields.io/badge/About-0d1117?style=for-the-badge&logo=readme&logoColor=58a6ff)](#about)
[![Projects](https://img.shields.io/badge/Projects-0d1117?style=for-the-badge&logo=github&logoColor=58a6ff)](#featured-projects)
[![Skills](https://img.shields.io/badge/Skills-0d1117?style=for-the-badge&logo=gnubash&logoColor=58a6ff)](#technical-skills)
[![Contact](https://img.shields.io/badge/Contact-0d1117?style=for-the-badge&logo=maildotru&logoColor=58a6ff)](#contact)

</div>

---

<table align="center">
  <tr>
    <td align="center"><b>AISEEF 2026</b><br/><sub>Gold Medalist<br/>Physics, Energy & Engineering</sub></td>
    <td align="center"><b>Nuclear Physics Club</b><br/><sub>Chairman<br/>University of Jember</sub></td>
    <td align="center"><b>Kibo-RPC 7th</b><br/><sub>Team Leader of Jatra<br/>JAXA programming challenge</sub></td>
    <td align="center"><b>REIVER Team</b><br/><sub>Team Leader<br/>Robotics R&D, UNEJ</sub></td>
  </tr>
</table>

---

## About

I am a Physics student at the University of Jember. I use fundamental physics as the starting point for computational research and for building hardware that measures, senses, and moves.

My academic interests are **nuclear physics, reactor physics, computational physics, and materials physics**. On the technical side I work on **robotics, embedded systems, instrumentation, and applied machine learning**. My research direction sits where the two meet: reactor modeling, radioisotope production, and simulation-driven analysis on one side, and hardware prototyping on the other.

```text
$ whoami
bfox8623 :: physics student
$ focus --list
  nuclear reactor modeling · scientific computing · instrumentation · robotics · embedded ML
```

## Research & Technical Interests

| Area | What I work on |
|---|---|
| **Nuclear & Reactor Physics** | Monte Carlo neutron transport, criticality (k-eff) analysis, depletion and isotope production, radioisotopes for targeted alpha therapy |
| **Computational Physics** | Simulation workflows, parallel computing environments, FEA, scientific visualization |
| **Instrumentation** | Force/pressure measurement, sensor calibration, measurement system analysis (MSA, Gage R&R) |
| **Robotics & Embedded Systems** | ESP32 control, autonomous robot programming, power electronics for robots |
| **Machine Learning (exploratory)** | Sensor data classification, deployment on resource-constrained microcontrollers |

---

## Featured Projects

### Th-232-Doped UN–PuN Gas-Cooled Fast Reactor for Ac-225 Production
`OpenMC 0.15.3` · `ENDF/B-VIII.0` · `Python` · **AISEEF 2026 Gold Medalist**

A **computational** study of a thorium-doped uranium–plutonium nitride (UN–PuN) gas-cooled fast reactor, investigating its potential for producing Actinium-225 for targeted alpha therapy.

```mermaid
flowchart LR
    A["Fuel and material<br/>modeling<br/>UN-PuN + Th-232"] --> B["Nuclear data<br/>ENDF/B-VIII.0"]
    B --> C["Monte Carlo<br/>neutron transport"]
    C --> D["Criticality<br/>k-effective"]
    D --> E["Depletion<br/>simulation"]
    E --> F["Ac-225 production<br/>vs. power configuration"]
    classDef core fill:#0d1117,stroke:#58a6ff,color:#e6edf3;
    class A,B,C,D,E,F core;
```

- Reactor material and fuel composition modeling
- Monte Carlo neutron transport and k-effective criticality analysis
- Depletion simulation and isotope production analysis
- Effect of power configuration on Ac-225 production

**My contribution:** reactor modeling and neutronic simulations.

> [!IMPORTANT]
> Simulation-based research only. No physical reactor was built or operated.

---

### Abdominal Tonometer with Embedded ML Exploration
`ESP32 / ESP32-C3` · `FSR402` · `ADC` · `Python` · `C/C++`

An instrumentation physics project: a pressure measurement approach based on controlled indentation depth, for studying abdominal muscle guarding (*defans muskular*).

```mermaid
flowchart LR
    A["FSR402 probe<br/>controlled indentation"] --> B["ESP32 ADC<br/>signal processing"]
    B --> C["Calibration<br/>known mechanical loads"]
    C --> D["Force to pressure<br/>kPa"]
    D --> E["MSA and<br/>Gage R&R"]
    D -.-> F["Features: max, min, avg kPa"]
    F -.-> G["ESP32-C3 lookup-table<br/>inference (exploration)"]
    classDef core fill:#0d1117,stroke:#58a6ff,color:#e6edf3;
    classDef explore fill:#0d1117,stroke:#8b949e,color:#8b949e,stroke-dasharray: 4 3;
    class A,B,C,D,E core;
    class F,G explore;
```

- FSR402-based probe, ADC signal processing, calibration with known mechanical loads
- Force-to-pressure conversion in kPa, probe design, and measurement methodology
- Ongoing: dataset preprocessing, feature engineering, and lookup-table-based classification inference on the ESP32-C3 Super Mini

> [!NOTE]
> A research and measurement prototype. Not a validated clinical or diagnostic device. Dashed boxes are ongoing exploration.

---

### Kibo-RPC: Autonomous Robot Programming and System Integration
`JAXA Kibo-RPC` · `Python` · `Docker` · `ROS 2 (exploration)`

Team Leader in the JAXA Kibo Robot Programming Challenge.

```mermaid
flowchart LR
    A["Robot programming"] --> B["Web-based<br/>simulation testing"]
    B --> C["Control and<br/>system integration"]
    C --> D["Troubleshooting<br/>communication and control"]
    D --> A
    C -.-> E["ROS 2 Jazzy + Docker<br/>(exploration)"]
    classDef core fill:#0d1117,stroke:#58a6ff,color:#e6edf3;
    classDef explore fill:#0d1117,stroke:#8b949e,color:#8b949e,stroke-dasharray: 4 3;
    class A,B,C,D core;
    class E explore;
```

ROS 2 Jazzy simulation in Docker was explored for future development and is not a completed integration.

<div align="center">

<a href="https://github.com/bfox8623/kibo">
  <img src="https://github-readme-stats.vercel.app/api/pin/?username=bfox8623&repo=kibo&theme=github_dark&bg_color=0d1117&hide_border=true&title_color=58a6ff&icon_color=58a6ff" alt="kibo repository" />
</a>

</div>

---

<details>
<summary><b>Additional exploration</b> (expand)</summary>

<br/>

- **AI and physics-informed learning (exploratory):** studying AI-driven rocket engine geometry generation (PicoGK, CFD, regenerative cooling) and a latent physics-informed neural network in PyTorch for hidden-state discovery in circuit simulation.
- **Reverse engineering and CTF practice:** binary exploitation and cryptography challenges with GDB and GEF.
- **Open-source IC design workflow:** exploring Yosys and Verilog.

</details>

---

## Technical Skills

<div align="center">

<img src="https://skillicons.dev/icons?i=py,c,cpp,arduino,pytorch,linux,arch,bash,vim,git,github,docker&theme=dark" alt="skills" />

</div>

<br/>

Levels reflect depth of project experience, not formal certification.

| Domain | Working With | Familiar With / Project Experience |
|---|---|---|
| **Computational Physics** | OpenMC, Python | Neutron transport, depletion analysis, reactor modeling, ANSYS FEA |
| **Programming** | Python, C/C++ for embedded targets | C (structured self-study) |
| **Embedded Systems** | ESP32, ESP32-C3, Arduino framework | UART, I2C, ADC, OLED interfaces, PCB power design |
| **Robotics** | Robot programming and control | Kibo-RPC, hardware integration, system troubleshooting |
| **Machine Learning** | Dataset preprocessing, feature engineering | Model training, embedded ML deployment (exploratory) |
| **Scientific Computing & Tools** | Git/GitHub, Arch Linux | Docker, OpenMPI, OpenMP, NFS, SSH, tmux |

---

## Currently Exploring

| Track | Focus |
|---|---|
| **Embedded ML** | Sensor classification inference on ESP32-C3 |
| **Robotics software** | ROS 2 Jazzy simulation environments with Docker |
| **HPC for nuclear sim** | Hybrid MPI/OpenMP parallelization for OpenMC workloads |
| **Low-level computing** | C programming (`kernel-journey/c-journey`) |
| **Hardware design** | Open-source IC design tooling (Yosys, Verilog) |

---

## GitHub Statistics

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=bfox8623&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=58a6ff" alt="GitHub stats" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=bfox8623&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff" alt="Top languages" />

<img src="https://streak-stats.demolab.com?user=bfox8623&theme=github-dark-blue&hide_border=true&background=0d1117" alt="Streak" height="150" />

<img src="https://github-readme-activity-graph.vercel.app/graph?username=bfox8623&bg_color=0d1117&color=58a6ff&line=1f6feb&point_color=e6edf3&area=true&area_color=1f6feb&hide_border=true" alt="Contribution activity" width="95%" />

</div>

---

## Contact

<div align="center">

[![Email](https://img.shields.io/badge/Email-your--email@example.com-0d1117?style=for-the-badge&logo=gmail&logoColor=58a6ff)](mailto:alrizyad@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-your--handle-0d1117?style=for-the-badge&logo=linkedin&logoColor=58a6ff)](https://linkedin.com/in/your-handle)
[![Instagram](https://img.shields.io/badge/Instagram-your--handle-0d1117?style=for-the-badge&logo=instagram&logoColor=58a6ff)](https://instagram.com/your-handle)

<br/>

<sub>Exploring the intersection of fundamental science, computational research, and real-world technological development.</sub>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:1f6feb&height=70&section=footer" alt="footer" width="100%" />

</div>
