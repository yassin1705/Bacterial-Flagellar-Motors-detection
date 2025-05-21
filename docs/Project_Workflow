Project Workflow
====================
Data Preprocessing:

Normalize tomogram slices.

Align slices to correct for drift.

Segmentation with U-Net:

Segment bacterial bodies in each 2D slice.

Membrane Detection with YOLO:

Detect membrane regions in each 2D slice.

Motor Localization:

Combine segmentation and detection outputs to estimate motor positions.

3D Position Averaging:

Track detected positions across adjacent slices.

Compute mean coordinates to consolidate detections and avoid duplicates.

