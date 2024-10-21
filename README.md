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

- **Objective**: This project calculates the flight path and photo locations for aerial photography surveys based on input parameters such as coordinates, camera types, and flight purposes.
- **Features**:
  - A graphical user interface (GUI) for inputting survey parameters.
  - Outputs include:
    - Flight path coordinates (`coordenadasvoo.txt`).
    - Graphical representation of the flight plan (`graficoplanovoo.png`).
    - Google Earth `.kml` file of the flight plan (`planovoo.kml`).
- **Dependencies**: `tkinter`, `matplotlib`, `math`, `utm`, `simplekml`, `shapely`

### 2. Photogrammetric Point Determination (Project2)

- **Objective**: This project uses MATLAB to determine the location of photogrammetric points based on image coordinates, internal and external orientations, and coordinate transformations.
- **Methodology**:
  - Uses orientation data and transformation matrices to compute accurate photogrammetric points.
  - Includes visual outputs of the computed points for further analysis.

## Folder Structure

- `/Project1/`: Folder containing the following files:
  - `coordenadasvoo.txt`: Example flight coordinates result
  - `dadosvoo.txt`: Alternative input file to bypass GUI
  - `flightplan.py`: Python code for flight path calculation
  - `graficoplanovoo.png`: Example graphic of the flight plan
  - `planovoo.kml`: Example Google Earth flight path
  - `README.txt`: Description of dependencies and code exceptions
- `/Project2/`: Folder containing the following files:
  - `/Code/`
    - `coordinates.m`: MATLAB code for photogrammetric points
    - `result.txt`: Example result output
    - `Proj2X0Y0.png`: Example graphic result
  - `/Data/`: Folder containing input data
- `presentation.pdf`: Presentation covering both projects and aditional classwork

## Conclusion

This repository showcases key aspects of photogrammetric workflows, from flight planning for aerial surveys to the determination of precise photogrammetric points using MATLAB and Python. Each project highlights a different element of photogrammetry, providing a comprehensive view of the techniques covered in this course.
