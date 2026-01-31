# Polar Stereo Vision Wave Reconstruction

This repository presents a stereo vision–based system for **3D sea surface reconstruction and significant wave height (Hs) inversion** in the Arctic Ocean, using shipborne binocular imagery acquired during a polar scientific expedition.

## 🌊 Project Background
Wave observation in polar regions is challenging due to complex sea states, sea ice coverage, extreme illumination conditions, and platform motion. Traditional instruments such as buoys and radar systems are costly or difficult to deploy in the Arctic.

This project develops a **vision-based alternative**, capable of reconstructing the 3D wave surface and estimating wave parameters from stereo images captured on a moving research vessel.

## 🚢 Data Source
- Platform: *Zhong Shan Da Xue Ji Di* Polar Research Vessel
- Region: Arctic Ocean
- Period: August – September 2024
- Sensors: Shipborne binocular cameras

Only **sample and processed data** are included in this repository due to data volume and usage restrictions.

## 🧠 Method Overview
The pipeline consists of the following stages:

1. **Image preprocessing**
   - Undistortion and rectification
   - Contrast enhancement (CLAHE)

2. **Feature extraction and matching**
   - SURF feature detection
   - Game-theoretic matching optimization
   - Epipolar constraint filtering

3. **Dense stereo reconstruction**
   - Semi-Global Matching (SGM)
   - 3D point cloud reconstruction

4. **Sea surface filtering and gridding**
   - RANSAC plane fitting
   - Regular grid interpolation (DCT-based)

5. **Wave parameter inversion**
   - Crest–trough detection
   - Significant wave height (Hs) estimation

## 📊 Experimental Results
- Successfully processed real shipborne data under complex Arctic sea conditions
- Overall wave level identification accuracy: **~75%**
- Strong correlation observed between:
  - Wind speed and wave height
  - Sea ice concentration and wave attenuation

## 📁 Repository Structure
# polar-stereo-wave-reconstruction
Stereo vision–based 3D wave surface reconstruction and significant wave height inversion in the Arctic Ocean using shipborne imagery.
