# Detecting Reproducible Fatal Collision Locations

This code implements the paper, Kim et al. (2021). Application of naïve Bayesian approach in detecting reproducible fatal collision locations on freeway. PLoS One 1–21. https://doi.org/10.1371/journal.pone.0251866

## Overview

The objective of the model is to detect reproducible fatal collision locations based on a naive Bayesian approach. We adopted continuous risk profile ([CRP](https://escholarship.org/uc/item/24m8j57d)) and spatial distribution of fatal collision locations as a prior and a likelihood, respectively. Based on the posterior that is the product of the prior and likelihood, reproducible fatal collision locations were detected and prioritized.

## Getting Started

### Dependencies
* R 4.0.3

### Components

#### Dataset
* 'Data' have the traffic crash data obtained from six routes of interstate highway in Californai from 2006 to 2008.
* Based on the data, Safety performance function (SPF) and continuous risk profile (CRP) were calculated and saved as separate files. For more details on calculating SPF and CRP, see [Kwon et al.(2013)](http://dx.doi.org/10.1016/j.aap.2012.10.019) and [Chung et al. (2009)](https://escholarship.org/uc/item/24m8j57d)

##### FatalCRP.R
* Step-by-step implementation is provided in this single file, including data preprocessing, modeling, evaluation, and visualization
* Refer the FatalCRP.html for a detailed description of the code  

## Notice
* Please refer to the full paper with this code for understanding the logic behind each process

## Authors

[@Eui-Jin Kim](https://sites.google.com/view/euijinkim)


## License

This project is licensed under the MIT License - see the LICENSE.md file for details

## Acknowledgments
* [Benchmark model](http://dx.doi.org/10.1016/j.aap.2012.10.019)
