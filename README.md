# Computer Vision Project End Course
## Title: MULTI-CLASS MEDICAL IMAGE SEGMENTATION WITH LACK OF LABELED DATA
Our repository is being updated day by day! The official code will be released soon!
# Getting started
### Requirements
Requirements are included in the requirement.txt.

### Data sets and pre-processing
Download:
1) [Combined Healthy Abdominal Organ Segmentation data set](https://chaos.grand-challenge.org/)
2) [Multi-sequence Cardiac MRI Segmentation data set](https://zmiclab.github.io/projects/mscmrseg19/) (bSSFP fold)

Pre-processing is performed according to [Ouyang et al.](https://github.com/cheng-01037/Self-supervised-Fewshot-Medical-Image-Segmentation/tree/2f2a22b74890cb9ad5e56ac234ea02b9f1c7a535) and we follow the procedure on their github repository.

Data-prepocessed is zipped in the folder: `dataloading` 
### Training
1. Download pretrained 3D ResNeXt weights. We use the pre-trained weights in `resnext-101-kinetics.pth` from [Hara et al.](https://openaccess.thecvf.com/content_cvpr_2018/papers/Hara_Can_Spatiotemporal_3D_CVPR_2018_paper.pdf) which is available on their [github repository](https://github.com/kenshohara/3D-ResNets-PyTorch). Note: Follow the link for the *old* pretrained weights. 
2. Processed-data uploaded in `dataloading` with `superdix.zip` and `chaos_MR_T2_normalized.zip`  
3. To view the detail implemented, run `few-shot-segmen.ipynb`
### Inference
Run `./script/test_<abd, cmr>_<2D, 3D>.sh` 
