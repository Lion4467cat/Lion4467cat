<div align="center">

# S. S. GOKULA SWAMY
### AI Systems Architect & Multimodal ML Researcher
**B.M.S. College of Engineering, Bengaluru** · *B.E. in Artificial Intelligence & Machine Learning (2023–2027)*  
**Sainik School Kodagu** · *NDA Written Qualified (Top ~0.5% nationwide) · NCC 'A', 'B', 'C' (Grade B)*

<br/>

<p align="center">
  <a href="https://lion4467cat.github.io/raikabuilds" target="_blank" rel="noopener noreferrer">
    <img src="https://img.shields.io/badge/Portfolio-raikabuilds-6366f1?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio" />
  </a>
  <a href="https://linkedin.com/in/ssgokulaswamy" target="_blank" rel="noopener noreferrer">
    <img src="https://img.shields.io/badge/LinkedIn-ssgokulaswamy-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:gokulaswamyss@gmail.com" target="_blank" rel="noopener noreferrer">
    <img src="https://img.shields.io/badge/Email-gokulaswamyss@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://github.com/Lion4467cat" target="_blank" rel="noopener noreferrer">
    <img src="https://img.shields.io/badge/GitHub-Lion4467cat-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
</p>

</div>

---

### ⚡ Architectural Focus
> **Engineering rigorous, spec-driven AI systems at the intersection of multimodal computer vision, zero-loop tensor optimization, and probabilistic decision-making.**  
> Specializing in multimodal visual metrology (SigLIP-2, DINOv2-S, MoGe-2, SAM 2.1), real-time acoustic signal forensics, and high-performance GPU-vectorized mathematical optimization.

---

## 🏆 Research & Competitive Accolades

```yaml
[RESEARCH PAPER] : Accepted at IEEE AIC 2026
Title            : "GPU-Accelerated Hybrid Two-Fidelity Genetic Algorithm for Wind Farm Layout Optimization on Irregular Polygon Domains"
Focus            : PyTorch GPU-vectorized Jensen wake model (zero Python loops) + conditional NREL FLORIS rescoring
Repository       : Lion4467cat/wflo-hybrid-ga

[HACKATHON]      : 1st Runner-Up (Team 39) — UNCLONE AI Hackathon 2026
Organizers       : BMSCE & DetectifAI (October 2026)
Project          : "Verified-Agent Badge" — Client-side real-time voice deepfake mitigation & stdlib audio forensics
Repository       : Lion4467cat/verified-agent-badge
```

---

## 🔬 Flagship Systems & Repositories

### 1. [`NutriSense`](https://github.com/Lion4467cat/NutriSense) — Autonomous 3D Dietary Metrology & PM POSHAN Statutory Auditing
*Single-photo institutional mid-day meal nutritional compliance pipeline combining 3D metric reconstruction with semantic mass regression.*
- **Perception & Segmentation**: Deployed **Google SigLIP-2 (768-dim)** with an $\alpha = 0.65$ soft background attenuation filter classifying 115 regional Indian dishes without food bleed.
- **3D Metric Geometry**: Reconstructed metric food volume via **Microsoft MoGe-2** metric depth paired with SVD tabletop annulus plane fitting ($3.5\text{ mm}$ tare deduction) and truncated conical liquid frustums.
- **Dual-Stream Mass Fusion**: Fused geometric volumes with a frozen **Meta DINOv2-S** SmoothL1 mass regression head using inverse-variance weighting ($w_{\text{geom}} \approx 0.27,\; w_{\text{head}} \approx 0.73$).
- **Statutory Audit Engine**: Evaluated macro/micronutrient compliance (IFCT 2017) via a **4,000-draw Monte Carlo engine** applying **Fréchet–Hoeffding comonotonic sums** to capture shared systematic errors; served via FastAPI with CUDA OOM guards to React 19.
- **Stack**: `PyTorch`, `FastAPI`, `React 19`, `SigLIP-2`, `DINOv2-S`, `MoGe-2`, `SAM 2.1`, `uv`, `Vite`.

---

### 2. [`wflo-ga`](https://github.com/Lion4467cat/wflo-hybrid-ga) — GPU-Accelerated Hybrid GA for Wind Farm Optimization
*Accepted Research Paper at IEEE AIC 2026.*
- **GPU Wake Vectorization**: Engineered a GPU-vectorized Jensen wake model in PyTorch executing $(8, 150, 150)$ tensor operations across 8 directional wind bins on irregular $10\text{ km} \times 10\text{ km}$ polygon domains with **zero Python loops** during candidate screening.
- **Two-Fidelity GA**: Screened candidates through vectorized Jensen wake physics, conditionally validating elite layouts through NREL FLORIS ($0.88$ fitness gate, 10-call per-generation budget cap).
- **Benchmark Gains**: Achieved **4029.16 GWh/yr** Annual Energy Production (**+2.69% / +105.7 GWh/yr AEP gain** over baseline, outperforming TOPFARM and Jensen-only GA) while strictly satisfying $\ge 400\text{ m}$ turbine spacing via tiered boundary repair operators.
- **Stack**: `PyTorch (CUDA Tensors)`, `FLORIS (NREL)`, `PyGAD`, `Shapely`, `TopFarm`, `PyWake`, `NumPy`.

---

### 3. [`Verified-Agent Badge`](https://github.com/Lion4467cat/verified-agent-badge) — Real-Time Voice Deepfake Defense & Acoustic Forensics
*1st Runner-Up at UNCLONE AI Hackathon 2026 (BMSCE & DetectifAI).*
- **Segment-Level Policy**: Built a client-side agent verifying banking representative authenticity in real time over 6-second live call buffers; enforces a segment-level policy where synthetic confidence $\ge 0.90$ on any 4-second chunk triggers an instant transaction hold, overriding reassuring call averages.
- **Zero-Dependency Signal Forensics**: Authored a pure Python standard-library PCM WAV forensics module detecting digital capture anomalies (silence tell $> 0.15$, room-tone RMS $< 0.004$, clipping).
- **Active Discrimination**: Implemented in-session Web Audio API pitch/spectral voice conversion for interactive live discrimination testing.
- **Stack**: `FastAPI`, `Python (stdlib Audio Forensics)`, `DetectifAI API`, `Web Audio API`, `Uvicorn`, `Render`.

---

### 4. [`The Greenifier`](https://github.com/Lion4467cat/greenifier) — Geospatial Rooftop Solar & Energy Auditor
*Automated end-to-end solar potential estimation and financial modeling from aerial satellite imagery.*
- **Geospatial Computer Vision**: Fetches keyless Zoom 18 satellite tiles via Web Mercator projection; segments usable roof planes and open terrain via OpenCV HSV color filtering, Canny edge suppression, and morphological closing.
- **LLM-Driven Financial Auditing**: Queries NASA POWER API for geographic solar irradiance and orchestrates Llama 3.3 70B (Groq) for automated financial modeling (system capacity, $\text{INR } 65,000/\text{kW}$ capex, payback timeline, $\text{CO}_2$ offset) through a responsive Leaflet.js and Flask dashboard.
- **Stack**: `OpenCV`, `Flask`, `NumPy`, `NASA POWER API`, `Llama 3.3 70B (Groq)`, `Leaflet.js`.

---

## 🛠️ Grounded Technical Stack

```
AI & Multimodal Vision  :: Google SigLIP-2 · Meta DINOv2-S · Microsoft MoGe-2 · Meta SAM 2.1 · Llama 3.3 70B
Numerical & Optimization :: PyTorch (CUDA Tensors) · NumPy · Shapely · PyGAD · FLORIS (NREL) · TopFarm · PyWake
Metrology & Forensics    :: SVD Plane Fitting · Inverse-Variance Fusion · Monte Carlo Comonotonic Sums · WAV Forensics
Backend & APIs           :: FastAPI · Flask · Uvicorn · DetectifAI API · NASA POWER API · Groq API
Frontend & Mapping       :: React 19 · Vite · Leaflet.js · Web Audio API · HTML5 · CSS3 · JavaScript (ES6+)
Engineering & Tooling    :: Linux · Git · GitHub · Docker · uv · Render
```

---

## ♟️ Off-Terminal: Endurance & Strategy
- **Cadet & Military Training**: Sainik School Kodagu alumnus. Qualified **UPSC NDA Written Examination 2023** (top ~0.5% nationwide). Earned **NCC Certificates 'A' (Grade A), 'B' (Grade B), and 'C' (Grade B)**. Awarded **Best Volunteer, NSS Annual Camp 2025** (selected from 100+ participants).
- **Endurance Athletics**: Completed **79.9 km and 58.2 km** timed endurance cyclothons, competitive marathon running, and high-altitude Himalayan trekking.
- **Strategy**: Competitive chess player applying calculation discipline to algorithm design.

---

<div align="center">
  <sub>Engineered with precision by <a href="https://github.com/Lion4467cat" target="_blank" rel="noopener noreferrer">S. S. Gokula Swamy</a> · Verified against ground-truth codebases</sub>
</div>
