1# GreenThumb
4BHITS Jahren Projekt- Benedikt Bliem/David Unterberger/Georg Schönerer
# Basic Idea
## Green house Simulator with Seasons and selling  
- **Core Loop:** 
	- Purchase seeds -> balance soil/climate -> harvest -> fulfill direct or wholesale orders -> reinvest profit
- **Platform Focus:**
	- PC/Tablet base physics engine
	- reserving VR for tactile minigames (pH calibration, pruning, stacking)
- **Environment Strategy:** 
	- Open field (low capital, high weather/pest risk, bulk crops)
	- Greenhouse (high setup/heating costs year-round high-value crops)
- **Seed Mechanics:** 
	- Budget standard seeds (resilient, lower profit)
	- premium hybrids (high yield, strict pH/NPK requirements)
- **Sales Channels:** 
	- Direct farm stand (high margin, low volume)
	- Wholesale semi-truck shipping (low margin, strict volume/deadline penalties)
- **Interactive Minigames:** 
	- Soil NPK/pH balancing
	- pest control choices (cheap chemical vs. organic tag)
	- produce quality sorting
- **Business Simulation:** 
	- Managing cash flow
	- equipment degradation
	- water access rights
	- seasonal market price fluctuations
	- and winter heating bills
# Weather Database
[Weather Dataset (2010–2026)](# Global Historical Weather Dataset (2010–2026))
```
Global-Weather-Dataset/
│
├── individual_cities/
│   ├── beijing.csv
│   ├── delhi.csv
│   ├── dubai.csv
│   ├── london.csv
│   ├── los_angeles.csv
│   ├── moscow.csv
│   ├── new_york.csv
│   ├── paris.csv
│   ├── phoenix.csv
│   ├── reykjavik.csv
│   ├── singapore.csv
│   └── tokyo.csv
│
├── merged_dataset/
│   └── Global_Weather_Dataset_2010_2026.csv
│
├── README.md
└── LICENSE

```


# GreenThumb – Technical Agro-Climatic & Weather Simulation Engine

## Project Overview
A data-driven greenhouse and open-field simulation engine focusing on regional climate impact, thermodynamic balance, and dynamic crop yield modeling using real-world historical weather data (2010–2026).

## Core Architecture
1. Weather Data Pipeline (ETL)
   - Ingestion of multi-region weather datasets (Beijing, London, Phoenix, etc.)
   - Time-series playback & acceleration (Temperature, Solar Radiation, Humidity, Precipitation)

2. Microclimate & Soil Physics Engine
   - Heat transfer & greenhouse energy balance calculation
   - Soil moisture dynamics & nutrient (NPK/pH) depletion algorithms

3. Crop Physiology Model
   - GDD-based growth modeling
   - Yield prediction under environmental stress vectors (frost, drought, nutrient deficiency)

4. Control Systems & Analytics
   - Automated climate control (HVAC, irrigation, shading)
   - Real-time telemetry dashboard & scenario comparative analysis