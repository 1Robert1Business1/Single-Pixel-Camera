# Single-Pixel Camera

A low-cost single-pixel camera prototype built with an RGB sensor, Arduino, 
and stepper motors, paired with a MATLAB simulation for image reconstruction 
using compressive sensing.

## Overview

Conventional cameras use millions of pixels to capture an image simultaneously. 
A single-pixel camera does the opposite — it captures one measurement at a time 
using structured light patterns, then reconstructs the full image mathematically. 
This makes it viable for imaging beyond the visible spectrum where traditional 
sensors are expensive or impractical.

## How it works

1. A sequence of optimised light patterns is projected onto the scene
2. A single RGB sensor records the reflected intensity for each pattern
3. Lasso regression (compressive sensing) reconstructs the original image 
   from the raw measurements
4. A MATLAB simulation validates the approach before physical construction

## Results

- Simulation achieved near-perfect image reconstruction accuracy
- Physical prototype successfully captured recognisable low-resolution images 
  within hardware budget constraints

## Stack

MATLAB · C · Processing · Arduino

## Structure

- `simulation/` — MATLAB simulation code and image reconstruction pipeline
- `hardware/` — 3D printed component files for the physical prototype
- `docs/` — Full project report

## Background

BEng Final Year Project — University of Kent (Distinction)
