# Conformal_Prediction_DSM

Implementation of conformal prediction as an uncertainty quantification method for soil organic carbon estimation. 
<!--
![Conformal_Prediction_DSM](./readme_imgs/cp_github.png)
-->
## Usage

1. To access the LUCAS topsoil dataset (ground truth), visit: [LUCAS Topsoil Dataset](https://esdac.jrc.ec.europa.eu/content/topsoil-physical-properties-europe-based-lucas-topsoil-data)
2. For the base code to download remote sensing images and climate data (input features for ML models), please refer to: [SoilNet GitHub Repository](https://github.com/moienr/SoilNet)

Once you have prepared the inputs and outputs (soil organic carbon - SOC in g/kg), save them as a .csv file.

3. The provided notebook contains functions to reproduce the experiments outlined in the paper. To run them, you need to install the Conformalized Quantile Regression (CQR) package, available at: [CQR GitHub Repository](https://github.com/yromano/cqr).
In addition to the required packages of CQR, also install `statsmodels`.

```bash
    conda install anaconda::statsmodels
```
