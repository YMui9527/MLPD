# MLPD: Multi-modal Lightning Prediction Dataset

## Overview

The **Multi-modal Lightning Prediction Dataset (MLPD)** is a comprehensive spatiotemporal dataset for lightning nowcasting research, integrating three heterogeneous data sources from Shandong Province, China:

- **RADAR**: Dual-polarization Doppler weather radar (CREF, ET, VIL)
- **LIG**: Lightning location system data
- **AWS**: Automatic Weather Station (Temperature, Humidity, Wind Speed)

This dataset supports the paper: *"ST-GLNet: A Spatiotemporal Graph Learning Network for Accurate Lightning Prediction Using Multimodal Meteorological Data"*.

Dataset is available at https://github.com/YMui9527/MLPD.git.

## Dataset Structure

```
MLPD/
├── AWS/          # Automatic Weather Station data
│   ├── RHU/      # Relative Humidity (.npy)
│   ├── TEM/      # Temperature (.npy)
│   └── WIN_S_Max/# Maximum Wind Speed (.npy)
├── LIG/          # Lightning observations (*_truth)
└── Radar/        # Dual-polarization radar data
    ├── CREF/     # Composite Reflectivity (.npy)
    ├── ET/       # Echo Top (.npy)
    └── VIL/      # Vertical Integrated Liquid (.npy)
```

## Dataset Specifications

| Attribute           | Details                                                      |
| ------------------- | ------------------------------------------------------------ |
| Study Area          | Shandong Province, China (34°25'N–38°23'N, 114°36'E–122°43'E) |
| Time Period         | August 2022 - October 2024                                   |
| Spatial Resolution  | 4 km × 4 km (113 × 177 grids)                                |
| Temporal Resolution | 1 hour                                                       |
| File Format         | NumPy arrays (.npy)                                          |
| File Naming         | `YYYYMMDDhh.npy` or `YYYYMMDDhh00_truth`                     |

**Current Available Data**: April - June 2024

⚠️ **Note**: Data from other months is being organized and will be uploaded soon.
