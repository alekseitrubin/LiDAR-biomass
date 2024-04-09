Processing of LiDAR laz files to create Canopy Height Model and generate trees and bushes shapefiles for biomass estimation

# LiDAR-Based Biomass Analysis (LiDAR-biomass)

## Project Overview
This project provides a solution to estimate biomass area based on vegetation analysis using LiDAR data. The script processes LiDAR .laz data to create a Canopy Height Model and generate trees and bushes shapefiles, allowing for an accurate assessment of biomass.

## Features
- Processing LiDAR data using CloudCompare from terminal (silent mode)
- Differentiating between trees and bushes based on height data
- Calculating the area covered by trees and bushes

## Prerequisites
Before running the script, ensure you have CloudCompare installed

## Usage
The process involves several steps, starting with LiDAR data processing in CloudCompare and followed by further analysis and shapefile generation.

1. **CloudCompare Steps:**
   - Export coordinates to SFs
   - Apply SOR, Noise and Cloth Simulation Filter (CSF)
   - Rasterize ground and off-ground points

2. **Python Workflow:**
   - Generate a Canopy Height Model
   - Perform raster calculations
   - Extract and dissolve cells for bushes and trees coverage
   - Calculate the area and generate the final shapefiles

## Output
- Bushes coverage shapefile
- Trees coverage shapefile
