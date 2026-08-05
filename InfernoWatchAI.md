# 🔥 InfernoWatchAI  
### **From Orbit to Alert in Seconds.**  
**Open-Source U.S. Wildfire Detection Platform Using Satellite Intelligence + Advanced AI**

---

## 🌎 Overview

**InfernoWatchAI** is a national-scale, open-source wildfire detection and intelligence system for the United States.  
Inspired by Australia’s world-leading wildfire platforms, this project integrates:

- Real-time satellite data  
- Thermal anomaly detection  
- AI smoke analysis  
- Multi-sensor fusion  
- Fire spread forecasting  
- Public dashboards & APIs  

All software is licensed under **AGPL 3.0+**, with required attribution to **Roxanne Ardary** and **roxanneardary.com** as specified in Section 7.

---

# 🚀 Key Features

## 🔭 1. Real-Time Satellite Fire Detection
Uses multiple satellite systems for high-precision detection:
- **GOES-16 / GOES-18** (5–10 min refresh)  
- **VIIRS** (high-resolution thermal anomalies)  
- **MODIS** (global daily imaging)  
- **Landsat** (optional high-res confirmation)

---

## 🔥 2. Multi-Sensor Fusion
Combines data from:
- Infrared satellite bands  
- Thermal anomalies  
- AI smoke signatures  
- Lightning strike data  
- Fuel dryness & vegetation maps  
- Weather conditions (humidity, wind, temperature)

This produces a **Confidence Score** for every detection.

---

## 🔥 3. AI Thermal Anomaly Detection
Neural models identify:
- Early-stage ignition points  
- Nighttime fires  
- Hidden hotspots  
- Industrial false positives (filtered automatically)

---

## 🌫️ 4. AI Smoke Detection & Plume Tracking
Vision Transformer model for:
- Smoke plume segmentation  
- Forecast drift paths  
- Air quality impact zones  
- Fire confirmation

---

## 🔮 5. Fire Growth & Spread Forecasting
Predictive modeling includes:
- Short-term (1–6 hour) projection  
- Weather-driven spread  
- Terrain + slope factors  
- Fuel dryness modeling  
- ConvLSTM and diffusion-based fire forecasting

---

## 🗺️ 6. Public Dashboard
Dashboard displays:
- Live fire detections  
- Confidence levels  
- Smoke plumes  
- Satellite layers  
- Weather overlays  
- Time-lapse playback  
- Historical trends  

---

## 📡 7. Open API
### **REST Endpoints**
- `/fires/live`  
- `/fires/history`  
- `/fires/confidence`  
- `/smoke/plumes`  
- `/risk/today`  

### **WebSockets**
- `/stream/fires`  
- `/stream/smoke`

---

## 🧪 8. Examples
Located in `/examples/`:
- Python Quickstart  
- JavaScript live map integration  
- CLI daily fire report generator  

---

## 📚 9. Historical Fire Intelligence
Includes datasets and analysis for:
- 15+ years of VIIRS/MODIS data  
- Fire clusters  
- Ignition frequency by region  
- Multi-year spread trends  
- Environmental correlations  

---

# 🧠 Architecture Summary

## 🛰️ Data Pipeline
1. Satellite Ingestion  
2. Preprocessing  
3. Spectral Band Extraction  
4. Heat Anomaly Detection  
5. Smoke Segmentation  
6. Multi-Sensor Fusion  
7. Confidence Scoring  
8. Alert Publication  

## 🧩 System Components
- **AI Models** (hotspot, smoke, false-positive filter, spread forecast)  
- **API Layer** (REST + WebSockets)  
- **Dashboard** (map viewer with layers)  
- **Data Storage** (time-series fire DB)

---

# 🔐 Confidence Scoring

- **Low** – Possible heat source  
- **Medium** – Likely wildfire  
- **High** – Confirmed wildfire (thermal + smoke alignment)

---

# 🌬️ Smoke Intelligence

The smoke module provides:
- Real-time plume mapping  
- Forecasted drift paths  
- Air quality risk zones  
- Hazard radius estimates  

---

# 🧭 Roadmap (Highlights)

- Mobile app for public alerts  
- Predictive burn modeling  
- Lightning-ignition correlation  
- State-level emergency integrations  
- Wildland-urban interface (WUI) maps  
- Multi-day spread projections  

See **ROADMAP.md** for the complete plan.

---

# 🤝 Contributing

Contributions are welcome!  
Please read the following before opening PRs:

- **CONTRIBUTING.md**  
- **CODE_OF_CONDUCT.md**

---

# 🛡️ Security

To report a vulnerability, follow the process described in **SECURITY.md**.

---

## Specification Branding License (SBL)
### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/infernowatchai/](https://roxanneardary.com/infernowatchai/)

---

# 📜 License & Notice Requirements

**InfernoWatchAI** is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- **InfernoWatchAI** specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
