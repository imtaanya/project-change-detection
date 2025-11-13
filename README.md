# Sentinel Data Automation

This repository provides Python scripts to **automatically download Sentinel-1 and Sentinel-2 products** from the Copernicus Data Space. It supports filtering by aoi, date, and product type, and downloads the data locally for further analysis.


## **Features**

- Query Sentinel-1 or Sentinel-2 products for a specific **Area of Interest (AOI)** and date range.
- Filter by parameters such as **cloud cover**, **product type**, etc.
- Automatically download **MSIL2A products** (Sentinel-2 Level-2A) or Sentinel-1 products.
- Skips already downloaded files to avoid duplication.


---
## Overview

This project automates the process of detecting and mapping palm plantations using Sentinel-2 imagery.
The workflow covers data download, preprocessing, vegetation index computation, filtering, and polygon extraction into a reproducible end-to-end pipeline.

# Install Dependencies
   pip install -r requirements.txt

## Data Download

1. To download Sentinel-1 imagery, use the `automate_sentinel_1_download.py` script.
2. To download Sentinel-1 imagery, use the `.automate_sentinel_2_download.py` script

This script:
1. Searches for Sentinel-2 **L2A** products (these are atmospherically corrected and have less cloud cover).
2. Displays the **top 10 matching products**.
3. Searches for Sentinel-2, Filter for GRD dataset and then start download

# Assumptions and Limitations

1. Add username and password in config, For sentinel-1, add the data range that you want to download.
2. Add the date range for downloading sentinel-2 data in `automate_sentinel_2_download.py`

   