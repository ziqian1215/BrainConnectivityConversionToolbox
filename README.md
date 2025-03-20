# Brain Connectivity Conversion Toolbox

## Overview
This repository contains the **Brain Connectivity Conversion Toolbox**, a framework designed to facilitate the transformation of connectivity matrices between different brain parcellation schemes. By leveraging continuous brain connectivity models, this toolbox enables neuroscientists to standardize connectome analyses and enhance reproducibility across studies.

## Features
- Converts structural connectivity (SC) matrices between **50+ parcellation schemes**.
- Supports **high-resolution SC reconstruction**.
- Provides **cross-atlas consistency validation**.
- Integrates with **Graph Neural Networks (GNNs)** for machine learning applications.
- Includes **visualization and comparison tools** for connectivity matrices.

## Installation
To use the toolbox, clone this repository and install the required dependencies:

```bash
git clone https://github.com/your_username/BrainConnectivityConversionToolbox.git
cd BrainConnectivityConversionToolbox
pip install -r requirements.txt
```

## Usage
### 1. Convert a Connectivity Matrix
```python
from conversion_toolbox import convert_connectivity
converted_matrix = convert_connectivity(input_matrix, source_atlas='Desikan', target_atlas='Schaefer100')
```

### 2. Validate Conversion Accuracy
```python
from evaluation import compute_correlation
correlation = compute_correlation(original_matrix, converted_matrix)
print(f"Conversion Correlation: {correlation:.4f}")
```

### 3. Visualize Connectivity Matrices
```python
from visualization import plot_connectivity
plot_connectivity(original_matrix, title='Original SC Matrix')
plot_connectivity(converted_matrix, title='Converted SC Matrix')
```

## Supported Atlases
The toolbox supports a variety of parcellation schemes, including:
- **Desikan-Killiany (68 regions)**
- **Destrieux (148 regions)**
- **Brainnetome (210 regions)**
- **Schaefer (100-1000 parcels)**
- **Yeo 7/17 Networks**
- **Gordon, Glasser (HCP-MMP1), CoCoNest Atlases**

## Applications
- **Standardizing connectivity analyses across studies**.
- **Enhancing reproducibility in network neuroscience**.
- **Pre-processing data for Graph Neural Network (GNN) models**.
- **Comparing connectivity measures across parcellations**.

## Citation
If you use this toolbox in your research, please cite:

```
```

## License
This project is licensed under the **MIT License** – see the `LICENSE` file for details.

## Contact
For questions or issues, please open an **Issue** on GitHub or contact:
**[Ziqian Zhang]** – zziqian092@gmail.com
