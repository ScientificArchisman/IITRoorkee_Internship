
# IIT Roorkee Internship Selection Project
---

**Student Name:** Archisman Chakraborti  
**Place of Study:** Harish Chandra Research Institute, Prayagraj
**Email:** archismanninja@gmail.com


## Overview
This project involves analyzing an EEG dataset obtained from [PhysioNet](https://physionet.org/content/eegmat/1.0.0/) and performing power spectral density (PSD) analysis. The dataset is used to train two deep learning models, EEGNET and ATCNET, to predict the group classification based on EEG signals.

## Dataset
The dataset used in this project is the "EEG During Mental Arithmetic Tasks" dataset, which is available on [PhysioNet](https://physionet.org/content/eegmat/1.0.0/).

## Analysis
### Power Spectral Density (PSD)
- PSD analysis was performed to understand the frequency components of the EEG signals.
- The PSD values were compared across different frequency bands (Delta, Theta, Alpha, Beta, Gamma) for both resting and task states.

### Models
#### EEGNET
- EEGNET is a convolutional neural network (CNN) designed specifically for EEG-based brain-computer interfaces.
- Reference: Lawhern, V. J., Solon, A. J., Waytowich, N. R., Gordon, S. M., Hung, C. P., & Lance, B. J. (2018). EEGNet: a compact convolutional neural network for EEG-based brain–computer interfaces. Journal of neural engineering, 15(5), 056013. DOI: [10.1088/1741-2552/aace8c](https://iopscience.iop.org/article/10.1088/1741-2552/aace8c)

#### ATCNET
- ATCNET is another deep learning model used for EEG signal classification.
- Reference: Zeng, H., Zhang, X., Zhang, Y., & Qin, Y. (2018). ATCNET: Attention-based Temporal Convolutional Network for Brain-computer Interface. arXiv preprint arXiv:1811.02990. DOI: [10.1109/TNNLS.2020.3012639](https://ieeexplore.ieee.org/document/9166687)

## Results
- Both EEGNET and ATCNET were trained on the dataset to predict the group classification.
- Initial performance showed an accuracy of 50%, likely due to the small number of samples (36 only).
- Further improvements can be achieved using cross-validation and hyperparameter tuning.

## Usage
To replicate this analysis, follow these steps:
1. Clone the repository:
   ```sh
   git clone https://github.com/ScientificArchisman/IITRoorkee_Internship.git
   ```
2. Install the required dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the analysis scripts:
   ```sh
   python analyze_psd.py
   python train_models.py
   ```

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments
We acknowledge the use of the PhysioNet database for providing the EEG dataset used in this analysis.

