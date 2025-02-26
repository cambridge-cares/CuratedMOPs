# MOP Assembler Data

This repository contains data files for the automated construction of metal–organic polyhedra (MOPs) and analogous cluster inorganics, as described in the technical report **Automated Assembly Modelling of Metal–Organic Polyhedra (c4e-Preprint Series 329)**.

## Contents

- **`input.csv`**  
  Lists MOP IDs, corresponding assembly models, and references to the chemical and generic building units (CBUs/GBUs).

- **`CBUs/`**  
  JSON files defining atomic coordinates, connectivity, and metadata for individual chemical building units. Each file provides the spatial fragment needed for MOP assembly.

- **`Assembly_Models/`**  
  A JSON file (`assembly_models.json`) specifying the geometric arrangement (positions, symmetries, and “dummy” atoms) for each assembly model.

## Usage

1. **MOP Construction**  
   The MOP assembler reads `input.csv` to identify which CBUs and assembly model should be combined.

2. **CBU Placement**  
   Each CBU’s coordinates and binding sites (“dummy” atoms) are matched to the relevant positions in the specified assembly model.

3. **Resulting Structures**  
   The output is a complete 3D structure suitable for geometry optimizations or high-throughput property estimations.

## Reference

Please cite the following report if you use this data:

> **Kondinski et al. (2024).** *Automated Assembly Modelling of Metal–Organic Polyhedra.*  
> Technical Report 329, c4e-Preprint Series, Cambridge.

For more details, see [The World Avatar](https://github.com/cambridge-cares/TheWorldAvatar) knowledge infrastructure.
