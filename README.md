# Multi-Type-Road-Surface-Dataset-MTRSD

This repository provides a **Multi-Type-Road-Surface-Dataset** for road surface recognition tasks, including six road surfaces with ambient illuminance data and encompassing structured and unstructured road surfaces. The dataset is designed to support supervised classification of different road surface types under varying illumination conditions.

---

## 1. Dataset Overview

The dataset consists of RGB road surface images collected under real-world lighting conditions. Each image is associated with:

* A **road surface category label** (derived from the filename prefix)
* An optional **illumination value** encoded in the filename

The dataset supports illumination-aware preprocessing and grayscale–RGB fusion for robust road surface recognition.

### Supported Road Surface Categories

| Class Tag | Class ID | Description             |
| --------- | -------- | ----------------------- |
| AP        | 0        | Asphalt Pavement        |
| CP        | 1        | Cement Pavement         |
| ES        | 2        | Earth Surface           |
| GS        | 3        | Grass Surface           |
| GGS       | 4        | Grass Gravel Surface    |
| GES       | 5        | Grass Earth Surface     |

---

## 2. Directory Structure

The dataset directory is organized as follows:

```
root_path/
├── AP/
│   ├── AP_01/
│   │    ├── AP_0001_illumination.jpg
│   │    ├── AP_0002_illumination.jpg
│   │    ├── AP_0003_illumination.jpg
│   │    └── ...
│   ├── AP_02/
│   ├── ...
│   └── AP_10/
├── CP/
│   ├── CP_01/
│   │    ├── CP_0001_illumination.jpg
│   │    ├── CP_0002_illumination.jpg
│   │    ├── CP_0003_illumination.jpg
│   │    └── ...
│   ├── CP_02/
│   ├── ...
│   └── CP_10/
├── ...
├── GGS/
└── GES/
```

Image filenames must follow the format:

```
<ClassTag>_<SequenceNumber>_<IlluminanceValue>.jpg
```

The **first character** defines the class label, and the **last numeric field** represents the illumination value.

---

## 3. License

This dataset and code are released for **academic and research use only** with license **CC BY 4.0**.

If you use this dataset in your research, please cite the corresponding paper or project.
