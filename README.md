# Photogrammetry Class Projects

**Institution**: Faculdade de Ciências da Universidade de Lisboa  
**Course**: Photogrammetry  
**Project Date**: 2021  
**Project Language**: Portuguese  

## Table of Contents

- [Overview](#overview)
- [Projects](#projects)
  - [1. Flight Path Calculator (Project1)](#1-flight-path-calculator-project1)
  - [2. Photogrammetric Point Determination (Project2)](#2-photogrammetric-point-determination-project2)
- [Folder Structure](#folder-structure)
- [Conclusion](#conclusion)

## Overview

This repository contains the projects developed for the Photogrammetry class. The projects focus on the automation of flight path planning for aerial photogrammetry surveys and the determination of photogrammetric points using coordinate transformations and orientation parameters.

## Projects

### 1. Flight Path Calculator (Project1)

- **Objective**: The goal of this project is to automate the flight path and photo location planning for aerial photogrammetry surveys. By entering key survey parameters (e.g., area coordinates, camera specifications, and flight purpose), the program generates a detailed flight plan.
  
- **Key Features**:
  - A **Graphical User Interface (GUI)** built using `tkinter` for intuitive input of survey parameters.
  - Generates flight path data:
    - **Flight path coordinates** in text format (`coordenadasvoo.txt`).
    - **Graphical representation** of the flight path (`graficoplanovoo.png`).
    - **Google Earth (.kml)** file for 3D visualization of the flight plan (`planovoo.kml`).
  - Provides flight parameters such as overlap percentages, the number of photos, flight time, and cost estimations.
  - Supports **custom cameras** by allowing manual input of camera specifications when predefined models aren't suitable.

- **Technology & Techniques**:
  - Python for all calculations and file generation.
  - Geospatial libraries: `utm` for coordinate conversion, `shapely` for geometry calculations, and `simplekml` for generating KML files.
  - Outputs include both 2D visualizations (using `matplotlib`) and 3D flight paths viewable in Google Earth.

- **Dependencies**:  
  Ensure the following Python libraries are installed: `tkinter`, `matplotlib`, `math`, `utm`, `simplekml`, `shapely`.

### 2. Photogrammetric Point Determination (Project2)

- **Objective**: This project calculates the 3D terrain coordinates of new photogrammetric points based on measurements from two aerial photographs forming a stereoscopic pair. It utilizes internal and external orientation data and coordinate transformation techniques to determine precise ground positions.

- **Key Features**:
  - **Orientation Calculations**: Uses MATLAB to compute the external orientation of photo 6, based on known ground control points (GCPs) and internal camera parameters.
  - **Point Triangulation**: Applies the Direct Spatial Intersection method to calculate the coordinates of new points from image coordinates across both photos.
  - **Iterative Adjustment**: Implements a least squares method to adjust the orientation and point positions for higher precision.
  - **Result Outputs**: Generates results that include both the final terrain coordinates and intermediary calculations (external orientation, image point residuals, etc.).

- **Technology & Techniques**:
  - MATLAB for numerical computation and geometric transformations.
  - Direct spatial intersection methods for photogrammetry.
  - Error minimization using the least squares method to refine results iteratively.
  - Visual outputs displaying the computed points and error metrics.

## Folder Structure

- `Photogrammetry/`
  - `/Project1/`
    - `coordenadasvoo.txt`: Example flight coordinates result
    - `dadosvoo.txt`: Alternative input file to bypass GUI
    - `flightplan.py`: Python code for flight path calculation
    - `graficoplanovoo.png`: Example graphic of the flight plan
    - `planovoo.kml`: Example Google Earth flight path
    - `README.txt`: Description of dependencies and code exceptions
  - `/Project2/`
    - `/Code/`
      - `coordinates.m`: MATLAB code for photogrammetric point determination
      - `result.txt`: Example result output
      - `Proj2X0Y0.png`: Example graphic result
    - `/Data/`: Folder containing input data
  - `presentation.pdf`: Presentation covering both projects and additional classwork

## Conclusion

This repository showcases key aspects of photogrammetric workflows, from the automated planning of aerial survey flight paths to the calculation of precise ground coordinates using photogrammetric point determination methods. Through these projects, users can gain insight into essential techniques used in photogrammetry, with practical applications using both Python and MATLAB.

