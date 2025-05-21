Workflow Overview
=================

The goal is to localize bacterial flagellar motors across cryo-tomograms using AI.

Steps:
------

1. **Preprocessing**
   - Normalize and align tomogram slices.

2. **Annotation**
   - Label motors manually or semi-automatically.

3. **Modeling**
   - Segment bacterial body using **U-Net** (per slice).
   - Detect membranes using **YOLO** (per slice).
   - Fuse outputs to estimate motor locations.

4. **Postprocessing**
   - Track detected motors across slices.
   - Compute **mean position** to avoid duplicates in 3D space.
