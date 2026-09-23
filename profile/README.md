<div align="center">

<img src="https://raw.githubusercontent.com/AUTONOMOUS-PCC-Inc/.github/main/profile/assets/banner.svg" alt="AUTONOMOUS PCC — Fisheye · LiDAR · V2X · Sensor Fusion" width="100%">

### Where GPS can't reach, vehicles drive themselves off the ship.

In GPS-denied zones aboard car carriers (PCC) and across port terminals,<br>
we automate **unmanned unloading and parking** of autonomous vehicles with fisheye–LiDAR fusion positioning.

[![Website](https://img.shields.io/badge/Website-autonomouspcc-0B1B33?style=flat-square)](https://d89yicdpi4w1g.cloudfront.net) [![Domain](https://img.shields.io/badge/Field-Ship%20%26%20Port%20Autonomy-1E6FD9?style=flat-square)](#) [![TRL](https://img.shields.io/badge/TRL-4~5-16A34A?style=flat-square)](#) [![Patents](https://img.shields.io/badge/Patents-3%20registered-7C3AED?style=flat-square)](#)

<br>

<img src="https://raw.githubusercontent.com/AUTONOMOUS-PCC-Inc/.github/main/profile/assets/hero.gif" alt="LiDAR point cloud fly-through of a parking structure" width="100%">

<sub>A parking structure reconstructed from real LiDAR point clouds — perceiving space from infrastructure alone, no GPS required.</sub><br>
<sub>▶ [Watch the original video (MP4)](https://d89yicdpi4w1g.cloudfront.net/videos/hero.mp4)</sub>

</div>

---

## Why Now

Autonomous vehicle exports are growing fast, yet **the last leg — loading onto and off the ship — is still done by hand**.

| Problem | Details |
|---|---|
| **GPS goes dark** | The thick steel hull and cramped decks of PCC vessels block satellite signals. Conventional GNSS-based autonomous driving simply stops working. |
| **Every car sees differently** | Tesla relies on vision, BYD on LiDAR — perception stacks vary by manufacturer, so no single-method control system can handle every model. |
| **The steering wheel disappears** | Level 4+ fully autonomous vehicles have no steering wheel. Having drivers move and park them by hand will soon be impossible. |

> We solve this by making the **infrastructure** smart, not the vehicle.
> Regardless of vehicle specs, the port and onboard infrastructure computes each car's position and sends it the route.

---

## What We Build

<div align="center">
<img src="https://raw.githubusercontent.com/AUTONOMOUS-PCC-Inc/.github/main/profile/assets/architecture.svg" alt="Architecture: infra fisheye and LiDAR fuse into a positioning engine driving V2X control" width="100%">
</div>

### 5 Core Technologies

| # | Technology | Description |
|:--:|---|---|
| 1 | **Fisheye 2D–2D Image Fusion** | Precisely matches infrastructure fisheye footage with the vehicle's around-view monitor (AVM) imagery to localize vision-based vehicles. Distortion-corrected training data ensures detection with no blind spots. |
| 2 | **2D–3D Camera–LiDAR Sensor Fusion** | Combines infrastructure visual data with 3D LiDAR point cloud (PCD) maps to obtain high-precision spatial coordinates for LiDAR-based vehicles. |
| 3 | **GPS-Denied Precision Positioning** | Hybrid infrastructure-based control achieves indoor positioning error within 30.5 cm inside ships and ports where signals are blocked. |
| 4 | **V2X Infrastructure Control** | Bidirectional vehicle–infrastructure communication and SDV (software-defined vehicle) integration let the infrastructure orchestrate the entire loading and unloading process. |
| 5 | **Fusion Training Datasets** | Builds and labels fisheye (2D) and LiDAR (3D) fusion data in standard COCO, YOLO, and PCD formats, with faces and license plates fully anonymized. |

### Solutions

- **Vision Positioning** — Fisheye-based 2D–2D vision localization
- **Sensor Fusion** — Unified 2D–3D camera–LiDAR perception
- **Autonomous Unloading** — Unmanned unloading automation for ships and ports
- **Digital Twin PMS** — Digital-twin-based parking optimization

---

## Numbers

<div align="center">
<img src="https://raw.githubusercontent.com/AUTONOMOUS-PCC-Inc/.github/main/profile/assets/metrics.svg" alt="98% detection precision, 30.5cm positioning error, 67% faster unloading, 40% lower cost" width="100%">
</div>

By reducing reliance on expensive LiDAR and leveraging low-cost fisheye infrastructure, we cut installation and operating costs by 40%+ compared with conventional positioning methods.

---

## Tech Stack

**Perception & Fusion**<br>
`Python` · `PyTorch` · `OpenCV` · `YOLO` · `Open3D` · `PCL` · `ROS 2`

**Simulation & Validation**<br>
`CARLA` · `AWSIM` · `Autoware`

**Vehicle & Embedded**<br>
`AUTOSAR` · `SDV` · `V2X` · `C/C++` · `On-Device AI`

**Standards**<br>
`ISO 26262` (Functional Safety) · `ISO 21448` (SOTIF) · `COCO` / `YOLO` / `PCD`

---

## Repositories

Our repositories are organized around the following areas.

| Area | Scope |
|---|---|
| **Perception** | Fisheye distortion correction, object detection, 2D–2D matching pipeline |
| **Fusion & Localization** | Camera–LiDAR calibration, PCD registration, indoor positioning engine |
| **Control & V2X** | Path tracking, vehicle–infrastructure communication, SDV interface |
| **Dataset Tools** | Labeling and QA tools, anonymization, standard format converters |
| **Simulation** | Validation of heterogeneous vehicle control algorithms on CARLA / AWSIM |
| **Web** | Company website (Vite + React + Tailwind) |

> Some repositories are kept private to protect intellectual property and under partner agreements.

---

## Milestones

| Date | Milestone |
|---|---|
| **2026.06** | Selected for the Data Voucher Program — Ministry of Science and ICT |
| **2026.05** | Selected for the Startup-Centered University Program — Ministry of SMEs and Startups |
| **2025.12** | Encouragement Award, AICOSS Industry–Academia Collaboration Project Competition |
| **2025.10** | Selected for the Pre-Startup Package (Deep Tech) — Ministry of SMEs and Startups |
| **2025.03** | Selected for the Korea I-Corps (K-ICorps) Program — Ministry of Science and ICT |
| **2024.12** | Grand Prize & Popularity Award, SEEK SQUARE 2024 |
| **2024.11** | Finalist (5th place), Embedded Software Contest |
| **2024.07** | Excellence Award, ABEEK Portfolio Competition |
| **2024.06** | Finalist (4th place), AWS Smart City Hackathon |

---

## Capability

- A dedicated **team of 7** specializing in autonomous driving and embedded systems
- Prototype at **TRL 4–5**
- Heterogeneous vehicle control algorithms validated on **CARLA · AWSIM**
- **3 registered patents**, including autonomous mobility path tracking, with an additional filing planned for fusion-data-based localization

---

## Roadmap

- [x] Fisheye-based indoor positioning prototype (error within 30.5 cm)
- [x] Simulation validation of control algorithms for vehicles with heterogeneous sensors
- [ ] Build and release 2D–2D / 2D–3D fusion training datasets
- [ ] Field demonstration of an integrated operating system at a port testbed
- [ ] Advance control algorithms to ISO 26262 / 21448 standards
- [ ] Expand SaaS control services to global PCTC operators

---

## Open Data

Autonomous driving training data for GPS-denied environments — ship interiors, underground parking garages — is nearly nonexistent in Korea.
We plan to **open part of our fusion datasets to research institutes and academia** to help advance Korea's self-reliance in autonomous driving technology.

- Fisheye (2D) and LiDAR (3D) fusion data with JSON/XML metadata labels
- Standard autonomous driving formats (COCO / YOLO / PCD)
- Released only after anonymizing personal data such as faces and license plates (blurring and masking)
- Integration with Korea's Public Data Portal and an open API planned

---

## Contact

<div align="center">

**AUTONOMOUS PCC, Inc.** · (주)오토노머스피씨씨

Field · Autonomous unmanned unloading for ships & ports / precision positioning<br>
Tech · Fisheye–LiDAR fusion datasets · V2X control

[![Email](https://img.shields.io/badge/Email-2170004487b%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:2170004487b@gmail.com)
[![Website](https://img.shields.io/badge/Website-Visit-0B1B33?style=for-the-badge)](https://d89yicdpi4w1g.cloudfront.net)

We welcome inquiries about technical collaboration, pilot partnerships, and careers.

</div>
