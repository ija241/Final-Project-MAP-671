# Park Accessibility in Lexington, Kentucky

## Project Overview

This project maps park accessibility in Lexington, Kentucky by showing areas within estimated walking distances of public parks. The goal is to identify which parts of the city have better access to green space and which areas may be underserved.

Public parks provide important environmental, recreational, and social benefits. However, access to these spaces is not always evenly distributed. This map visualizes accessibility using distance-based walking zones to highlight spatial inequalities in access.

---

## Data Sources

The following datasets were used in this project:

- Parks data – [Boundaries of city and state maintained parks within Lexington-Fayette County, Kentucky.](https://data.lexingtonky.gov/)
- Streets data – [road network used for spatial context](https://data.lexingtonky.gov/)
---

## Methods

This map was created using QGIS following these steps:

1. **Data Import**
   - Loaded parks and streets shapefiles into QGIS.

2. **Projection Setup**
   - Set the project coordinate reference system (CRS) to a projected system to NAD 83/ Kentucky Single Zone.


4. **Buffer Creation**
   - Created buffer zones around parks to represent walking accessibility:
     - 400 meters (~5-minute walk)
     - 800 meters (~10-minute walk)
   - Dissolved buffers to create continuous accessibility areas.

5. **Map Styling**
   - Parks were styled in green.
   - Accessibility zones were symbolized using graduated shades of green with transparency.
   - All the data layers were designed in a way that it creates a visual contrast
   - The background was set to dark green to match the overall theme of greenspace

6. **Map Layout**
   - Designed the final map in the QGIS Print Layout.
   - Added essential elements:
     - Title
     - Legend
     - Scale bar
     - North arrow
     - Metadata (author, projection, data source)

7. **Export**
   - Exported the final map as two static images:
     - A smaller version (1200 px width) for web display
     - A larger version (8000 px width) for download

---

## Projection

The original data projection was checked in QGIS.

The final map was projected using:

**[ NAD83 / Kentucky Single Zone]**

---

## Final Map

View the project webpage here:

👉 [Insert your GitHub Pages link here]

---

## High Resolution Map

Download the full-resolution map:

👉 [Insert link to your 8000px image here]

---

## Repository

Access the full project files here:

👉 [Insert your GitHub repository link here]

---

## Why This Map Was Created

This map was created to explore spatial differences in access to public parks in Lexington. By visualizing walking distance zones, the project highlights areas that may benefit from improved park access or future planning efforts.

---

## Reflection

**What went well:**
The use of multiple datasets (parks, streets, and bufferzones) helped create a clear and informative map. The buffer-based approach effectively communicates accessibility in a simple and understandable way. 

**What could be improved:**
Future work could incorporate network-based analysis using actual walking paths instead of straight-line distance buffers, which would provide a more realistic representation of accessibility. Also adding building data and showing which builtup areas are closer or farther from parks
