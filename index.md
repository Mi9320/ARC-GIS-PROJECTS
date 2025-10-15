# 🛢 Oil Spill Risk and Ecosystem Sensitivity Mapping – Puget Sound, Washington

## 🌍 Project Overview
This project identifies areas of **high environmental risk** in Puget Sound, Washington, where **oil spills from tanker routes** may impact sensitive ecosystems.  
The analysis integrates shipping lane data with ecosystem layers such as wetlands, marine protected areas (MPAs), and habitats for threatened fish species including Chinook Salmon, Rockfish, and Boccaccio.

---

## 🎯 Objectives
- Map **high-risk oil spill zones** around tanker shipping routes.  
- Determine which **ecosystems and species habitats** overlap with these risk areas.  
- Quantify the **extent (km²)** of affected regions to support environmental management and emergency response planning.  

---

## 🗺️ Study Area
**Puget Sound**, located in northwestern Washington State, is a critical marine ecosystem supporting commercial shipping, fisheries, and recreation.  
It is home to **ESA-listed species** and ecologically rich wetlands that are vulnerable to contamination from oil spills.

---

## 🍀 Data Sources
| Dataset                              | Source                               | Description                      |
|---------------------------------------|--------------------------------------|----------------------------------|
| Shipping Lanes / Tanker Routes        | NOAA Marine Cadastre                 | Maritime traffic corridors       |
| Wetlands                              | USGS National Wetlands Inventory (NWI)| Estuarine and freshwater wetlands|
| Fish Habitat (Chinook, Rockfish, Boccaccio) | NOAA Fisheries / WDFW              | Critical and essential fish habitat|
| Marine Protected Areas                | Washington Department of Ecology     | Protected coastal zones          |
| Hydrography / DEM                     | USGS                                 | Contextual reference layers      |

All data were projected to **WGS 1984 Web Mercator (Auxiliary Sphere)**.

## 🧠 Methodology and GIS Tools Used
| Step | Tool / Process           | Purpose                                                     |
|------|-------------------------|-------------------------------------------------------------|
| 1    | **Buffer**              | Created 2 km buffer around tanker routes to define risk zones|
| 2    | **Clip**                | Extracted layers within Puget Sound boundary                |
| 3    | **Erase**               | Removed land portions from buffer to keep only marine areas |
| 4    | **Intersect**           | Identified overlap between 2 km buffer and ecosystem layers |
| 5    | **Calculate Geometry**  | Computed area (km²) of affected features                   |
| 6    | **Summary Statistics**  | Summarized total risk areas by habitat or species           |
| 7    | **Merge**               | Combined summary tables into one unified dataset            |
| 8    | **Layout View**         | Designed thematic maps with titles, legends, and scale bars |
| 9    | **Inset Map**           | Added zoomed-out locator map for regional context           |
| 10   | **Share as Web Map**    | Published final results to ArcGIS Online and StoryMaps      |

## 📊 Results
- Generated **2 km oil spill risk zone** along all tanker routes.  
- Identified high-risk overlaps near **Seattle, Tacoma, and Whidbey Island**.  
- Found significant intersections between the buffer and:
  - Estuarine & marine wetlands  
  - Chinook salmon migration corridors  
  - Rockfish and Boccaccio essential habitats  
  - Several marine protected areas  

### Summary of Key Species at Risk
- **Chinook Salmon** – Threatened species; highly sensitive to oil exposure in estuarine and nearshore habitats.  
- **Rockfish** – Long-lived reef fish; vulnerable to habitat loss and contamination.  
- **Boccaccio** – Threatened rockfish; limited reproduction and high exposure to oil spill zones.

---

## 🗂️ Deliverables
- `PugetSound_OilSpillRisk.gdb` – Geodatabase with processed and intersected layers  
- `Wetlands_Risk_2km.pdf` – Wetlands at risk map layout  
- `Chinook_Risk_2km.pdf` – Salmon habitat risk map  
- `Rockfish_Risk_2km.pdf` – Rockfish habitat risk map  
- `MPA_Risk_2km.pdf` – Marine Protected Areas risk map  
- `PugetSound_LocatorMap.pdf` – Overview map  
- `Summary_Table.csv` – Area (km²) of affected ecosystems and species habitats  

---

## 🌐 Published Outputs
- [Download ArcGIS Pro Project Package (.ppkx)](https://drive.google.com/file/d/1rDM2wYOwI6aSd7hHsR_G7UW-n506B1Cd/view?usp=sharing)
- [High_Risk_Zones_for_Salmon_Chinook.pdf](https://github.com/user-attachments/files/22897985/High_Risk_Zones_for_Salmon_Chinook.pdf)
- [High_Risk_Zones_for_Rockfish_Yelloweye.pdf](https://github.com/user-attachments/files/22897984/High_Risk_Zones_for_Rockfish_Yelloweye.pdf)
- [High_Risk_Zones_for_Bocaccio.pdf](https://github.com/user-attachments/files/22897982/High_Risk_Zones_for_Bocaccio.pdf)
- [summary table.xls](https://github.com/user-attachments/files/22910347/summary.table.xls)

---

## 🧰 Technologies Used
- **ArcGIS Pro** – Data processing and map creation  
- **ArcGIS Online / StoryMaps** – Web publishing and visualization  
- **QGIS** – Data inspection and format conversion  
- **Python (ArcPy)** – Automated geometry calculations  
- **Excel / CSV** – Area summaries and reporting  

---

## 🧾 Conclusion
The analysis highlights **ecologically sensitive zones** most vulnerable to oil spills in Puget Sound.  
These findings can assist policymakers and environmental agencies in prioritizing **spill prevention and response efforts** while protecting threatened marine species and coastal habitats.

---

## 👤 Author
**Ibrahim Mirza**  
📍 Ottawa, Ontario, Canada  
📧 mirzaibrahim551@gmail.com  


---








**Contact:** [mirzaibrahim551@gmail.com]
