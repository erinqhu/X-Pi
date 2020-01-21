# Saved Trained Models
These models are saved for fast loading when we continue to work on the model training and for uploading to Flask or Raspberry Pi when we use the model remotely.

<br />

* ResNet50, stage 1
* ResNet50, stage 2
* Vgg16bn, stage 1
* Vgg16bn, stage 2
* Vgg16bn (PyTorch)

<br />

| Transfer Model Name | Additional Layers | # of Data Entries | Hyper Parameteres | Best Accuracy |
| :---: | :---: | :---: | :---: | :---: |
| ResNet50 | None | 50,000 | lr=3e-2 | 78.5% |
| ResNet50 | None | 50,000 | lr=slice(1e-5, 6e-3) | 78.8% |
| Vgg16bn | None | 50,000 | lr=2e-2 | 77.66% |
| Vgg16bn | None | 50,000 | lr=slice(1e-5, 4e-3) | 79.15% |
| Vgg16bn| None, modified the original 1,000 output classes to 14 | lr=1e-5 | 83% |
