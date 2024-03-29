# Conformal_Prediction_DSM

Implementation of conformal prediction as an uncertainty quantification method for soil organic carbon estimation. 

![Conformal_Prediction_DSM](./img/cp_github.png)

Please site: 

<pre>
@Article{rs16030438,
AUTHOR = {Kakhani, Nafiseh and Alamdar, Setareh and Kebonye, Ndiye Michael and Amani, Meisam and Scholten, Thomas},
TITLE = {Uncertainty Quantification of Soil Organic Carbon Estimation from Remote Sensing Data with Conformal Prediction},
JOURNAL = {Remote Sensing},
VOLUME = {16},
YEAR = {2024},
NUMBER = {3},
ARTICLE-NUMBER = {438},
URL = {https://www.mdpi.com/2072-4292/16/3/438},
ISSN = {2072-4292},
DOI = {10.3390/rs16030438}
}
</pre>

## Usage

1. To access the LUCAS topsoil dataset (ground truth), visit: [LUCAS Topsoil Dataset](https://esdac.jrc.ec.europa.eu/content/topsoil-physical-properties-europe-based-lucas-topsoil-data)
2. For the base code to download remote sensing images and climate data (input features for ML models), please refer to: [SoilNet GitHub Repository](https://github.com/moienr/SoilNet)

Once you have prepared the inputs and outputs (soil organic carbon - SOC in g/kg), save them as a .csv file.

3. The provided notebook contains functions to reproduce the experiments outlined in the paper. To run them, you need to install the Conformalized Quantile Regression (CQR) package, available at: [CQR GitHub Repository](https://github.com/yromano/cqr).
In addition to the required packages of CQR, also install `statsmodels`.

```bash
    conda install anaconda::statsmodels
```
4. In each iteration, the results will be saved as separate .csv files, and then you can use them to calculate the uncertainty and accuracy metrics.

This repository will be updated gradually. Meanwhile, do not hesitate to contact me via: nafiseh.kakhani@uni-tuebingen.de
