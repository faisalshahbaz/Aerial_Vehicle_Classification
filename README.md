## Aerial Vehicle Detection using Synthetic Images

This repository contains our work on `Aerial Vehicle Detection
using Synthetic Images`. You can find more details on our work in the
following paper :

	@inproceedings{uzkent2017tracking,
		Title={Tracking in Aerial Hyperspectral Videos using Deep Kernelized Correlation Filters},
		Author={Uzkent, Burak and Rangnekar, Aneesh and Hoffman, Matthew J},
		Journal={arXiv preprint arXiv:1711.07235},
		Year={2017}
	}

### Synthetic Training Dataset
The goal of our work is detect vehicles on the `WAMI` platform by using convolutional model trained on a synthetic vehicle detection dataset. Our synthetic dataset consists of `55226` images with vehicle and background samples and each image is represented by `48x48` pixels. The synthetic images are generated by the `Digital Imaging and Remote Sensing` Software (DIRSIG) owned by the `Chester F. Carlson Center for Imaging Science, Rochester Institute of Technology`. The synthetic scenes comes from the MegaScene-I area available in DIRSIG.The vehicular traffic simulation, on ther other hand, is generated by the `Simulation of Urban Mobility Platform` (SUMO) and coupled to DIRSIG. Some of the positive samples from our dataset is shown below.

![DIRSIG_Positives](./figures/DIRSIG_positives.jpg =500x500)

### Validation Dataset
To test the fidelity of the synthetic dataset, we validate the performance of the convolutional network, trained on the synthetic dataset, on the validation dataset containing the real vehicle and background images recorded with the `WAMI` platform. Our validation dataset consists of 600 images from the CLIFF06 and CLIFF07 datasets. Some of the positive images from the validation dataset can be visualized in the figure below.

![WAMI_Positives](./figures/WAMI_positives.jpg =500x500)

The goal of this study is to reduce the dependency on the WAMI dataset to train a convolutional network model. With our synthetic dataset, we believe that the `overfitting` to the a couple of datasets captured from the WAMI dataset is avoided. 

### Download Links

Download our aerial vehicle detection dataset

```
wget https://drive.google.com/open?id=1cQIM2a7gNaxlE2oFdQ_O-GqgBo84fLia
```

If you use our aerial vehicle detection dataset in your research project, please cite our paper :

	@inproceedings{uzkent2017tracking,
		Title={Tracking in Aerial Hyperspectral Videos using Deep Kernelized Correlation Filters},
		Author={Uzkent, Burak and Rangnekar, Aneesh and Hoffman, Matthew J},
		Journal={arXiv preprint arXiv:1711.07235},
		Year={2017}
	}

