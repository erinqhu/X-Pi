# Training Code with Different Pre-Trained Models
`pytorch_hackathon_cheXpert_rn50.ipynb`: import fastai package; train the dataset on ResNet50 architecture for two phases, phase 1 using fixed learning rate and phase 2 using sliced learning rates across layers.
`pytorch_hackathon_cheXpert_vgg16.ipynb`: very similar to the code above but using Vgg16bn architecture.
`cheXpert_pytorch_vgg16bn_gradcam_final.ipynb`: use PyTorch (not fastai) to build a customized Vgg16bn model; train the model and save the best model that has the highest average accuracy. predict output classes for test data using the best model; implement Grad-CAM on 10 best predicted images and eight worst predicted images for model future modification (explainable AI).
