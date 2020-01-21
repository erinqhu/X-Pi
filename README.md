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

## Best Result (so far)

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
