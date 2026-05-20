# Ambulance Response Time Jakarta

<p>
  <img src="https://img.shields.io/badge/Python-Jupyter_Notebook-3776AB?style=flat-square&logo=jupyter&logoColor=white" />
  <img src="https://img.shields.io/badge/Platform-Google_Colab-F9AB00?style=flat-square&logo=googlecolab&logoColor=white" />
  <img src="https://img.shields.io/badge/Visualization-Leaflet.js-199900?style=flat-square&logo=leaflet&logoColor=white" />
  <img src="https://img.shields.io/badge/Coverage-DKI_Jakarta-red?style=flat-square" />
</p>

A geospatial analysis of ambulance distribution, response time, and population coverage across DKI Jakarta. This project assesses the spatial adequacy of emergency medical services (EMS) in Jakarta using open administrative and operational data, visualized interactively via Leaflet.js.

---

## Research Questions

- How are ambulances spatially distributed across Jakarta's administrative areas?
- What is the average response time per district, and which areas are underserved?
- What is the ambulance-to-population ratio per kelurahan/kecamatan?
- Which areas fall outside ambulance service coverage zones?

---

## Repository Structure

```
Ambulance_Response_Time_Jakarta/
├── Data Ambulance Jakarta/          # Operational ambulance location and deployment data
├── Batas Wilayah Jakarta/           # Administrative boundary shapefiles for DKI Jakarta
├── Waktu Respon/                    # Response time data per district/area
├── Rasio Ambulan-Penduduk/         # Ambulance-to-population ratio analysis output
├── service area/                   # Service area / coverage zone spatial analysis
└── Leaflet Ambulance Google Collab.ipynb   # Main analysis & interactive map notebook
```

---

## Methodology

1. **Data Collection** — Ambulance location and response data collected from Jakarta's EMS records; administrative boundaries sourced from official GIS portals
2. **Spatial Analysis** — Service area modeling using network-based or buffer-based approaches to delineate coverage zones per ambulance station
3. **Response Time Analysis** — Statistical evaluation of response times per kelurahan and kecamatan, benchmarked against WHO emergency response standards
4. **Ratio Analysis** — Ambulance-to-population ratio calculated per administrative unit to identify areas with insufficient EMS capacity
5. **Visualization** — Interactive choropleth and point maps built with Leaflet.js, rendered in Google Colab

---

## Getting Started

### Run in Google Colab (Recommended)

Open the main notebook directly in Google Colab:

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zakiulfahmijailani/Ambulance_Response_Time_Jakarta/blob/main/Leaflet%20Ambulance%20Google%20Collab.ipynb)

### Run Locally

```bash
git clone https://github.com/zakiulfahmijailani/Ambulance_Response_Time_Jakarta.git
cd Ambulance_Response_Time_Jakarta

pip install pandas geopandas folium matplotlib
jupyter notebook "Leaflet Ambulance Google Collab.ipynb"
```

---

## Context

This project is part of a broader research initiative on **geospatial analysis of public health infrastructure in Indonesian urban areas**. Jakarta, as the most densely populated city in Indonesia, presents a critical case study for evaluating emergency service equity across heterogeneous administrative units.

The analysis contributes to ongoing work on:
- **SIGAPP** — Agentic GeoAI for Education Planning (NTT)
- Urban service adequacy benchmarking for Indonesian cities
- Open data utilization in public health geospatial research

---

## Contributing

Suggestions and improvements are welcome, particularly for:
- Network-based routing analysis (replacing buffer-based service areas)
- Integration with real-time ambulance tracking data
- Extension to other Indonesian cities

Open an [Issue](https://github.com/zakiulfahmijailani/Ambulance_Response_Time_Jakarta/issues) or contact: [zakiul.jailani@bakrie.ac.id](mailto:zakiul.jailani@bakrie.ac.id)

---

<p align="center">
  <sub>Geospatial analysis for equitable emergency services. Powered by open data.</sub>
</p>
