# Jae Kyung Yu (유재경)

**Cosmetic Formulation R&D Researcher** · Sun Care Specialist · Smart Manufacturing & Digital Twin

📍 Suwon, South Korea  ·  ✉️ jekee92711@naver.com

---

## 👋 About Me

Cosmetic formulation R&D researcher with **9+ years of experience** specializing in **sun care products**.
I bridge the gap between **formulation design** and **manufacturing process optimization**, and I'm now
extending that work into **physics-based digital twins** for data-driven smart manufacturing.

- 🧪 Expert in sunscreen formulation, UV protection (SPF/PA), and formulation stability
- ⚙️ Strong background connecting lab-scale formulation with mass-production processes
- 🤖 Building digital-twin & quality-prediction systems for cosmetic manufacturing
- 🎓 M.S. student in **Smart Factory Convergence (SKKU)**; led a population-balance-model (PBM) digital-twin capstone (**CEVSim**)
- 🔬 3 patents filed/registered in cosmetic composition technology

---

## 🛠️ Technical Skills

| Area | Details |
|------|---------|
| **Formulation** | Sunscreen emulsion · dispersion · stick formulation |
| **UV Testing** | In-vitro SPF & PA measurement |
| **Process Engineering** | Mixing · scale-up · process optimization |
| **Modeling & Simulation** | Population Balance Model (PBM) · Droplet Size Distribution (DSD) · equal-ε scale-up |
| **Smart Manufacturing** | Digital Twin · Three.js / WebGL 3D · process simulation · web deployment |

---

## 💼 Professional Experience

### Cosmecca Korea — *Principal Researcher, Sunscreen Formulation R&D*
`Jun 2017 – Present`

- Conducted formulation R&D of sunscreen products (emulsion, dispersion, stick types)
- Designed formulations balancing SPF/PA performance, stability, sensory properties, and regulatory requirements
- Improved reproducibility of sunscreen performance by optimizing key process variables (mixing speed, temperature, order of addition)
- Performed in-vitro SPF/PA evaluation and stability testing
- Transferred formulations from lab-scale to mass production, reducing quality variation
- Collaborated with production and quality teams to resolve manufacturing issues

---

## 🚀 Capstone Design Project — CEVSim `2026`

### Droplet-Distribution-Based Quality-Prediction Simulator for Cosmetic Manufacturing Vessels
*Smart Factory Capstone Design 1, Sungkyunkwan University · Team 12 — **Team Lead***

**Team:** Jae Kyung Yu (유재경, lead) · Min-gyu Kang (강민규) · Seo-woo Lee (이서우) · Hak-seung Lee (이학승)
**Advisor:** Prof. Jongpil Jeong (정종필)

A web-based **3D digital twin** of the dissolution tank and main vessel that makes the previously
unobservable internal emulsification process visible, and predicts the resulting product properties
**before manufacturing** using a population balance model (PBM).

**What it does**

- Renders the full process (dissolution tank → main vessel) in real-time 3D (Three.js / WebGL)
- A **65-node Fixed-Pivot PBM** predicts four quality metrics from a single droplet size distribution (DSD): **D₃₂ · H-Index · viscosity · hardness**
- **Three-tier QC auto-judgment** (PASS / REVIEW / FAIL) based on the number of failing metrics
- **Equal-energy-dissipation (equal-ε) scale-up** auto-derives recommended RPM for 100 / 300 / 500 L vessels — V-100: 2,500 · V-300: 1,958 · V-500: 1,748 rpm

**Implementation**

- 5 self-built modules — Physics · PBM engine (65-node) · Vessel3D · Dissolver3D · MiniChart — in a single ~4,000-line HTML application
- Dual calculation core (Calabrese ↔ PBM) running the 5-stage sequence: charge → dissolve → transfer → homogenize → QC
- Deployed on **GitHub Pages** (no install — runs in the browser)

**Results**

- Brought quality indicators from **1 → 4 metrics (4×)** via the dual core
- Inter-vessel **D₃₂ deviation ≤ 5%** under equal-ε scale-up
- 🔗 [Cosmetic-Emulsification-Vessel-Simulator](https://github.com/jekee711/Cosmetic-Emulsification-Vessel-Simulator-)

**Next steps:** quantitative validation with measured DSD/viscosity · CFD-PBM coupling for internal ε distribution · coalescence term · target-property inverse design

---

## 📚 Research Outputs

### Publication

**Scale-Up Simulation of Cosmetic Emulsion Manufacturing Vessels (100–500 L) Using a Population Balance Model: Integrated Multi-Metric Analysis of Droplet Size Distribution, Uniformity, Viscosity, and Hardness**
*Submitted to **ICSOC 2026** (International Conference on Service-Oriented Computing), Industry Track · 2026, under review — lead author*

> Proposes an integrated simulator that couples a 65-node Fixed-Pivot PBM quality-prediction engine to a
> full-process 3D visualization of a homomixer-equipped vessel. From recipe, impeller RPM, and vessel
> volume it derives the energy dissipation rate ε, time-evolves the DSD (RK4, 1000 s), and consistently
> derives four metrics (D₃₂, H-Index, viscosity, hardness) from a single DSD, then applies a three-tier QC
> auto-judgment (PASS / REVIEW / FAIL). The PBM mode yields **4× more quality metrics** than the
> single-metric Calabrese baseline, and an equal-ε scale-up guideline (N ∝ V⁻²ᐟ⁹) converges inter-vessel
> D₃₂ deviation across 100/300/500 L vessels to **within 5%**. Predictions were checked for industrial
> consistency against production-lot shipment viscosity and storage stability.

### Software Copyright

- **CEVSim — Cosmetic Emulsification Vessel Scale-Up Simulator** (화장품 에멀젼 제조 가마 스케일업 시뮬레이터)
  **Registered** ✅ — Computer Program Work copyright, Korea Copyright Commission (한국저작권위원회)
  Registration no. **C-2026-030853** (제C-2026-030853호) · Receipt no. 2026-032760 · Registered **2026-06-23**
  Registrant: Sungkyunkwan University Industry–Academic Cooperation Foundation (성균관대학교산학협력단)

### Patent *(project-derived)*

- **Method and System for Scale-Up Emulsification Quality Prediction and Judgment of Cosmetic Emulsion Manufacturing Vessels Using a Population Balance Model and Multiple Quality Metrics**
  (개체군 수지 모델과 다중 품질지표를 이용한 화장품 에멀젼 제조 가마의 스케일업 유화 품질 예측·판정 방법 및 시스템)
  Filed 2026-06-14 · application **R-2026-0578-KR-1** · representative inventor: Prof. Jongpil Jeong

---

## 🔎 Paper Reviews (Seminar)

In-depth analyses of published work that informed the capstone's PBM and digital-twin design.

**[Individual] CFD simulation of a high-shear mixer for food emulsion production**
*Ferrari, M., Boccardo, G., Buffo, A., Vanni, M., Marchisio, D. L. — Journal of Food Engineering 358, 111655 (2023) · presented 2026-03-24*

> A CFD–PBM digital-twin study of mayonnaise droplet breakup in a cone-mill high-shear mixer. It couples
> OpenFOAM CFD (2D/3D) of the non-Newtonian flow with a QMOM population balance model and extends the
> analysis beyond the rotor–stator gap to the pre-/post-mixing chambers, finding that **shear flow within
> the gap is the dominant breakage mechanism** — a physical basis for digital-twin process design.

**[Team 12] A population balance model for cosmetic emulsion design: A multiscale approach**
*Calvo, F., Gómez, J. M., Ricardez-Sandoval, L., Álvarez, O. — Chemical Engineering Science 287, 119737 (2024) · presented 2026-05-26*

> A multiscale PBM framework for cosmetic emulsion design that links operating conditions, formulation, and
> product properties across scales. It is the **first study to connect thickener concentration to PBM tuning
> parameters**, derives empirical correlations between DSD and rheology/texture/energy consumption, and
> demonstrates PBM integration into a model-based design strategy.

---

## 📄 Patents — Cosmetic Composition

- **Cosmetic composition with enhanced make-up color sustainability** — *2021, filed*
- **Low specific gravity W/O emulsion cosmetic composition** — *2021, registered*
- **Ceramide-based sunscreen composition and manufacturing method** — *2024, under review*

---

## 🧴 Selected Product Experience

- Developed multiple sunscreen and base makeup products for global brands
- Products launched in major retail channels including **Olive Young** and **Daiso**

---

## 🎓 Education

**Sungkyunkwan University (SKKU)**, South Korea — *M.S. in Smart Factory Convergence*
`In progress`

**Kyonggi University**, South Korea — *B.S. in Chemistry*
`2012 – 2016`

---

## 🌐 Languages & Certifications

| Language | Level | Certification |
|----------|-------|---------------|
| Korean | Native | — |
| English | Intermediate | TOEIC 805 |
| Chinese | Intermediate | HSK Level 5 (209) |
| Japanese | Basic | JPT 505 |

---

<sub>📫 Open to opportunities in cosmetic R&D, formulation science, and smart manufacturing.</sub>
