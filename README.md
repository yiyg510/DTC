## Dual-task Consistency
Code for this paper: Semi-supervised Medical Image Segmentation through Dual-task Consistency ([DTC](https://arxiv.org/pdf/2009.04448.pdf))
* More details and comparison methods will be released if the paper is accepted. 
* The multi-classes **DTC** is under doing, and also will be released as we finished it.
## Requirements
Some important required packages include:
* [Pytorch][torch_link] version >=0.4.1.
* TensorBoardX
* Python == 3.6 
* Some basic python packages such as Numpy, Scikit-image, SimpleITK, Scipy ......

Follow official guidance to install [Pytorch][torch_link].

[torch_link]:https://pytorch.org/

# Usage

1. Clone the repo:
```
git clone https://github.com/HiLab-git/DTC.git 
cd DTC
```
2. Put the data in [data/2018LA_Seg_Training Set](https://github.com/Luoxd1996/DTC/tree/master/data/2018LA_Seg_Training%20Set).

3. Train the model
```
cd code
python train_la_dtc.py or python train_la_dtc_v2.py
```

4. Test the model
```
python test_LA.py
```
Our best model is saved in the model dir [DTC_model](https://github.com/Luoxd1996/DTC/tree/master/model), and the pretrained SASSNet and UAMT model can be download from [SASSNet_model](https://github.com/kleinzcy/SASSnet/tree/master/model) and [UA-MT_model](https://github.com/yulequan/UA-MT/tree/master/model).

## Citation
If you find this repository is useful in your research, please consider to cite:

	@article{luo2020semi,
	  title={Semi-supervised Medical Image Segmentation through Dual-task Consistency},
	  author={Luo, Xiangde and Chen, Jieneng and Song, Tao and Chen, Yinan and Wang, Guotai and Zhang, Shaoting},
	  journal={arXiv preprint arXiv:2009.04448},
	  year={2020}
	}

## Acknowledgement
* This code is adapted from [UA-MT](https://github.com/yulequan/UA-MT), [SASSNet](https://github.com/kleinzcy/SASSnet), [SegWithDistMap](https://github.com/JunMa11/SegWithDistMap). 
* We thank Dr. Lequan Yu, M.S. Shuailin Li and Dr. Jun Ma for their elegant and efficient code base.
* More semi-supervised learning approaches for medical image segmentation have summarized in this repository [SSL4MIS](https://github.com/Luoxd1996/awesome-semi-supervised-learning-for-medical-image-segmentation).

