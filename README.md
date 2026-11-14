# S. S. Gokula Swamy

**AI & ML Researcher** · B.E. in Artificial Intelligence & Machine Learning at **B.M.S. College of Engineering**, Bengaluru (2023–2027)

Engineering deep learning systems across **3D multimodal visual metrology**, **GPU-vectorized mathematical optimization**, and **real-time audio signal forensics**.

<p>
  <a href="https://lion4467cat.github.io/raikabuilds" target="_blank" rel="noopener noreferrer"><img src="https://img.shields.io/badge/Portfolio-raikabuilds-1d3b72?style=flat-square&logo=googlechrome&logoColor=white" alt="Portfolio" /></a>
  <a href="https://lion4467cat.github.io/raikabuilds/assets/SS_Gokula_Swamy_Resume.pdf" target="_blank" rel="noopener noreferrer"><img src="https://img.shields.io/badge/Resume_%2F_CV-PDF-1d3b72?style=flat-square&logo=readme&logoColor=white" alt="Resume / CV PDF" /></a>
  <a href="https://linkedin.com/in/ssgokulaswamy" target="_blank" rel="noopener noreferrer"><img src="https://img.shields.io/badge/LinkedIn-ssgokulaswamy-1f2328?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:gokulaswamyss@gmail.com" target="_blank" rel="noopener noreferrer"><img src="https://img.shields.io/badge/Email-gokulaswamyss%40gmail.com-1f2328?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

---

| Publication | Hackathon | Academics | National Exam |
| :--- | :--- | :--- | :--- |
| **IEEE AIC 2026** (Accepted)<br/>[`wflo-hybrid-ga`](https://github.com/Lion4467cat/wflo-hybrid-ga) | **1st Runner-Up (Team 39)**<br/>UNCLONE AI 2026 · [`verified-agent-badge`](https://github.com/Lion4467cat/verified-agent-badge) | **7.37 / 10 CGPA**<br/>B.E. AIML, BMSCE Bengaluru | **UPSC NDA 2023**<br/>Written Qualified (Top ~0.5%) |

---

## 01 // Research Publication

**GPU-Accelerated Hybrid Two-Fidelity Genetic Algorithm for Wind Farm Layout Optimization on Irregular Polygon Domains**  
*Accepted at 2026 IEEE World Conference on Applied Intelligence and Computing (AIC 2026)* · [Repository (`Lion4467cat/wflo-hybrid-ga`)](https://github.com/Lion4467cat/wflo-hybrid-ga)

- **GPU Wake Vectorization:** Engineered a PyTorch GPU-vectorized Jensen wake model executing `(8, 150, 150)` tensor operations across 8 directional wind bins on irregular $10\text{ km} \times 10\text{ km}$ polygon domains with **zero Python loops** during candidate screening.
- **Two-Fidelity Surrogate Gating:** Screened layouts with fast vectorized Jensen wake physics and conditionally validated elite candidates through **NREL FLORIS** (`0.88` fitness gate, `10-call` per-generation budget cap) paired with tiered boundary repair enforcing $\ge 400\text{ m}$ turbine spacing.
- **Benchmark Gains:** Achieved **4029.16 GWh/yr** Annual Energy Production (**+2.69% / +105.7 GWh/yr** AEP gain over baseline, outperforming TOPFARM and Jensen-only GA).

---

## 02 // Selected Systems

| System | Domain | Core Stack |
| :--- | :--- | :--- |
| [`NutriSense`](https://github.com/Lion4467cat/NutriSense) | 3D Dietary Metrology & PM POSHAN Auditing | `SigLIP-2`, `MoGe-2`, `DINOv2-S`, `SAM 2.1`, `PyTorch`, `FastAPI`, `React 19` |
| [`Verified-Agent Badge`](https://github.com/Lion4467cat/verified-agent-badge) | Real-Time Voice Deepfake Defense *(1st Runner-Up, UNCLONE AI 2026)* | `FastAPI`, `Python stdlib`, `DetectifAI API`, `Web Audio API`, `Uvicorn` |
| [`The Greenifier`](https://github.com/Lion4467cat/greenifier) | Geospatial Rooftop Solar & LLM Energy Auditing | `OpenCV`, `Flask`, `NumPy`, `NASA POWER API`, `Llama 3.3 70B`, `Leaflet.js` |

### [`NutriSense`](https://github.com/Lion4467cat/NutriSense) — *3D Dietary Metrology & PM POSHAN Statutory Auditing*
Single-photo institutional mid-day meal nutritional compliance pipeline combining metric 3D reconstruction with semantic mass regression.
- **Segmentation & Classification:** Deployed **Google SigLIP-2 (768-dim)** with an $\alpha = 0.65$ soft background attenuation filter and **SAM 2.1**, classifying **115 regional Indian dishes** without food bleed.
- **3D Metric Geometry:** Reconstructed food volume via **Microsoft MoGe-2** metric depth, **SVD tabletop annulus plane fitting** ($3.5\text{ mm}$ tare deduction), and truncated conical liquid frustums.
- **Dual-Stream Mass Fusion:** Fused geometric mass estimates with a frozen **Meta DINOv2-S** SmoothL1 mass regression head using inverse-variance weighting ($w_{\text{geom}} \approx 0.27,\; w_{\text{head}} \approx 0.73$).
- **Statutory Audit Engine:** Evaluated macro/micronutrient compliance (**IFCT 2017**) via a **4,000-draw Monte Carlo engine** applying **Fréchet–Hoeffding comonotonic sums**; served over FastAPI (with CUDA OOM guards) to React 19.

### [`Verified-Agent Badge`](https://github.com/Lion4467cat/verified-agent-badge) — *Real-Time Voice Deepfake Defense & Acoustic Forensics*
*1st Runner-Up (Team 39), UNCLONE AI Hackathon 2026 (BMSCE & DetectifAI).*
- **Segment-Level Guardrail Policy:** Verifies caller voice authenticity over **6-second rolling call buffers**, enforcing an instant transaction hold whenever synthetic confidence reaches $\ge 0.90$ on any 4-second chunk (overriding reassuring call-level averages).
- **Zero-Dependency Signal Forensics:** Authored a pure **Python stdlib PCM WAV forensics** analyzer flagging digital capture anomalies (`silence tell > 0.15`, `room-tone RMS < 0.004`, amplitude clipping).
- **Active Discrimination:** Built in-session **Web Audio API** pitch and spectral conversion controls for live spoofing stress tests.

### [`The Greenifier`](https://github.com/Lion4467cat/greenifier) — *Geospatial Rooftop Solar & LLM Energy Auditor*
Automated rooftop solar siting and financial modeling pipeline from satellite imagery.
- **Geospatial Computer Vision:** Fetches keyless **Zoom 18 Web Mercator** satellite tiles and segments usable rooftop area with **OpenCV** (HSV thresholding, Canny edges, morphological closing).
- **LLM Energy Auditing:** Combines **NASA POWER** solar irradiance data with **Llama 3.3 70B (Groq)** to model system capacity, capex ($\text{INR } 65,000/\text{kW}$), payback period, and $\text{CO}_2$ offset in a **Flask** and **Leaflet.js** dashboard.

---

## 03 // Technical Stack

| Domain | Technologies |
| :--- | :--- |
| **ML & Computer Vision** | `PyTorch (CUDA)`, `SigLIP-2`, `DINOv2-S`, `MoGe-2`, `SAM 2.1`, `Llama 3.3 70B`, `OpenCV`, `NumPy`, `Monte Carlo Simulation` |
| **Optimization & Metrology** | `PyGAD`, `FLORIS (NREL)`, `PyWake`, `TopFarm`, `Shapely`, `SVD Plane Fitting`, `Inverse-Variance Fusion`, `PCM WAV Forensics` |
| **Backend & Web Systems** | `FastAPI`, `Flask`, `React 19`, `Vite`, `Leaflet.js`, `Web Audio API`, `Uvicorn`, `Groq API`, `NASA POWER API`, `DetectifAI` |
| **Languages & Tooling** | `Python`, `SQL`, `JavaScript (ES6+)`, `HTML5`, `CSS3`, `Git`, `GitHub`, `Linux`, `Docker`, `uv`, `Render` |

---

## 04 // Education, Credentials & Activities

| Category | Details |
| :--- | :--- |
| **B.M.S. College of Engineering** *(2023–2027)* | **B.E. in Artificial Intelligence & Machine Learning** · Bengaluru · **CGPA: 7.37 / 10** (7th Sem) |
| **Sainik School Kodagu** *(2016–2023)* | **CBSE Class XII:** 88.6% · **Class X:** 91.4% · Residential Cadet Schooling |
| **UPSC NDA (2023)** | Qualified Written Examination (placed in top ~0.5% nationwide) |
| **NCC & NSS** | **NCC Certificates ‘A’ (Grade A), ‘B’ (Grade B), and ‘C’ (Grade B)** · **Best Volunteer Award**, NSS Annual Camp 2025 (selected from 100+ participants) |
| **Certifications** | Python for Data Science *(IBM)* · Green Skills and AI *(Edunet Foundation)* |
| **Endurance & Hobbies** | Self-supported **79.9 km** and **58.2 km** endurance cycling rides; recreational marathon runner; high-altitude trekking *(hobby)*; competitive chess player |

---

<sub>Portfolio: <a href="https://lion4467cat.github.io/raikabuilds" target="_blank" rel="noopener noreferrer">lion4467cat.github.io/raikabuilds</a> · Resume: <a href="https://lion4467cat.github.io/raikabuilds/assets/SS_Gokula_Swamy_Resume.pdf" target="_blank" rel="noopener noreferrer">SS_Gokula_Swamy_Resume.pdf</a></sub>
