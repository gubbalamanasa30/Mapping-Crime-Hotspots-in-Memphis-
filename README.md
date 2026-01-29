# Mapping Crime Hotspots in Memphis (ArcGIS Pro)

A GIS project that analyzes and visualizes **crime hotspot patterns in Memphis, TN** using incident-level point data and spatial analysis techniques in **ArcGIS Pro**. The final output is a presentation-ready map exported as a high-quality PDF.

> **Deliverable:** `outputs/Memphis_Crime_Hotspots.pdf` (final map layout)  
> **Organization:** Center for Applied Earth Science and Engineering Research (CAESER)

---

## Project Overview

### Objective
Identify and visualize **areas with high concentrations of reported crime incidents** to support public safety discussions such as:
- Resource allocation and patrol planning
- Community safety prioritization
- Data-driven policy insights

### Key Outputs
- A crime incident map classified by **UCR Category**
- Hotspot visualization using **Kernel Density**
- Influence visualization using **Buffer zones**
- Exported **PDF map layout** titled **“Crime Hotspots in Memphis”**
---

## Methods & GIS Workflow (ArcGIS Pro)

### 1) Data Preparation
- Imported tabular crime incident data (e.g., incident type/category, location fields, severity if available).
- Converted incident records into spatial point features using **XY Table To Point** (points represent individual incidents).  
  *In the exported layout, the layer naming indicates an XY-to-point workflow.* 

### 2) Buffer Analysis
- Created **buffer zones** around incident points to represent localized influence areas.
- Buffers help interpret proximity clustering visually and support exploratory analysis. 

### 3) Kernel Density (Hotspot Surface)
- Ran **Kernel Density** to generate a continuous density surface (heatmap-like output) of crime concentration.
- High density areas represent **hotspots** for deeper investigation or planning use-cases. 

### 4) Cartography & Layout Design
The final layout includes:
- Clear map title: **Crime Hotspots in Memphis**
- Scale bar and basemap context
- Symbology and legend for **UCR Category** classes  
  (e.g., Aggravated Assault, Assault, Robbery, Motor Vehicle Theft, etc.) 
---

## Tools & Technology
- **ArcGIS Pro** (geoprocessing + cartography)
- Spatial analysis tools used:
  - XY Table To Point
  - Buffer
  - Kernel Density
    
