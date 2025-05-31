# Week 2 Report

## 1. Approach

Briefly describe your overall methodology for loading, processing, and visualizing the neuroimaging data. For example:

- **Data Loading**  
  - Used `nibabel` to load NIfTI files (`.nii`) into Python.  
  - Converted NIfTI volumes into individual DICOM slices using `pydicom` for further inspection and interoperability.

- **Metadata Extraction**  
  - Extracted key header information (shape, affine matrix, voxel spacing, data types) from NIfTI.  
  - Extracted DICOM tags (Patient Name, Study Date, Modality, Pixel Spacing, Slice Thickness, Image Position, etc.) to verify consistency and completeness.

- **Visualization**  
  - Displayed representative slices using `matplotlib` to confirm proper orientation and intensity ranges.  
  - Added annotations or overlays (e.g., scale bars, slice indices) to highlight specific features.

- **Workflow Outline**  
  1. Mount Google Drive (if necessary) and verify file paths under `/content/`.  
  2. Write a loop to load all five NIfTI files, print their basic metadata, and store them in a dictionary.  
  3. Convert each NIfTI volume to a folder of DICOM `.dcm` slices, ensuring correct pixel data type and minimal required tags.  
  4. Load a few of the generated DICOM files to extract and print their metadata.  
  5. Plot a couple of slices side by side to confirm that the conversion preserved orientation and intensity values.

---

## 2. Visualizations

Below, insert screenshots of the key plots you generated. You can add captions to clarify what each figure is showing.
   
**Figure : Axial|Coronal|Sagital Slice of sub-62038**  
![Axial Slice of sub-62038](image.png)

