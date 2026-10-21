# Cytoskeleton and Cell Morphology Analysis

## 1. Student Information
- **Student name:** Angela B. Villegas 
- **Selected Phenotype:** Large spread
- **Actin and DNA filenames:** 17301-actin.DIB & 17301-DNA.DIB 
- **Image Field ID:** 17301
- **BBBC018 download link:** https://bbbc.broadinstitute.org/BBBC018

---

## 2. Methods

### Fiji/ImageJ

1. Opened the actin fluorescence image in Fiji/ImageJ.
2. Opened the matching DNA image as a visual reference.
3. Selected five intact and clearly visible cells.
4. Traced each cell's outer boundary using the Freehand Selection tool.
5. Measured the area, mean fluorescence intensity, circularity, and aspect ratio.
6. Saved the measurements as `data/fiji_results.csv`.
7. Saved an annotated image showing the measured cells as `figures/measured_cells.png`.

### R Analysis

R was used to read the Fiji measurements and calculate the following summary statistics:

- Number of cells measured
- Mean cell area
- Mean circularity
- Mean aspect ratio
- Mean actin fluorescence intensity

Two graphs were generated: cell area versus circularity and actin fluorescence intensity.

## 5. Results

### Figure 1. Measured Cells
<img width="967" height="1018" alt="829" src="https://github.com/user-attachments/assets/a3f355b9-9aab-4509-b3ec-b9063b951deb" />

### Figure 2. Cell Area versus Circularity
<img width="1000" height="700" alt="area_vs_circularity" src="https://github.com/user-attachments/assets/50044834-5ee8-4d4f-b71b-f2a2caa5c46b" />

### Figure 3. Actin Fluorescence Intensity
<img width="1000" height="700" alt="actin_intensity" src="https://github.com/user-attachments/assets/f9c2f39e-ef45-4da2-a503-708d70f08100" />

## 6. Interpretation

### 1. What phenotype was observed, and what visible evidence supports the classification?

The selected phenotype was **Large spread**. This classification was based on the visible features of the cells in the actin fluorescence image, particularly cells that spread out and cover a larger area. I can use the cell area measurements and the image's appearance to help identify this phenotype.

### 2. Were the five cells mostly round or elongated?

Based on the measurements, the five cells were mostly round. The high overall average circularity of 0.842 (with cells 2, 3, and 5 exceeding 0.85) combined with a low average aspect ratio of 1.232 indicates that the majority of measured cells maintained a predominantly circular morphology.

### 3. What is the role of actin in cell shape and movement?

Actin helps maintain cell shape and supports cell spreading. It can also reorganize to help cells form extensions and move.

### 4. Why cannot one fixed image show cell movement speed?

A fixed image shows the cells at only one point in time, so it cannot show how fast they move. To measure movement speed, we need images of living cells taken at different times.
