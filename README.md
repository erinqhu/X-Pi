# X-Pi
Low cost solution to detect chest pathologies deployed to Raspberry Pi and Flask without radiologists

https://www.youtube.com/watch?v=QC-d8nf_SdA&feature=youtu.be

## Dataset
CheXpert is a large dataset of chest X-rays and competition for automated chest x-ray interpretation, which features uncertainty labels and radiologist-labeled reference standard evaluation sets. 
CheXpert is a large public dataset for chest radiograph interpretation, consisting of 224,316 chest radiographs of 65,240 patients.
https://stanfordmlgroup.github.io/competitions/chexpert/

## X-Pi: Model explanation
Here is a nice explanation by Qin (Erin) Hu regarding the X-Pi Model trained on ResNet50.

https://www.youtube.com/watch?v=DH-LfOf_ia4&feature=youtu.be

## Results

| Transfer Model Name | Additional Layers | # of Data Entries | Hyper Parameteres | Best Accuracy |
| :---: | :---: | :---: | :---: | :---: |
| ResNet50 | None | 50,000 | lr=3e-2 | 78.5% |
| ResNet50 | None | 50,000 | lr=slice(1e-5, 6e-3) | 78.8% |
| Vgg16bn | None | 50,000 | lr=2e-2 | 77.66% |
| Vgg16bn | None | 50,000 | lr=slice(1e-5, 4e-3) | 79.15% |
| Vgg16bn| None, modified the original 1,000 output classes to 14 | 48,000 (2,000 for test)| lr=1e-5 | 83% |

**Grad-CAM Results**

*100% predicted image*

Patient 12642: Lung Opacity, Pleural Effusion, Support Devices
<p float="left">
  <img src="results/grad-cam_results/best/patient12642_Lung Opacity.jpg" width="250" />
  <img src="results/grad-cam_results/best/patient12642_Pleural Effusion.jpg" width="250" /> 
  <img src="results/grad-cam_results/best/patient12642_Support Devices.jpg" width="250" />
</p>

*50% predicted image*

Patient 03462: Lung Opacity, Pleural Effusion, Support Devices
<p float="left">
  <img src="results/grad-cam_results/worst/patient03462_Lung Opacity.jpg" width="250" />
  <img src="results/grad-cam_results/worst/patient03462_Pleural Effusion.jpg" width="250" /> 
  <img src="results/grad-cam_results/worst/patient03462_Support Devices.jpg" width="250" />
</p>
