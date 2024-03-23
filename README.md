# WildFire-Detection-from-drones-footages
This repo contains a computer vision model to detect wildfires from drone's footages

This model was created to solve task 1 of G20 use case at Start Hack (an hackathon that takes place every year in St. Gallen).

## Model Architecture
We first performed Transfer Learning on EfficientNetB0 using the dataset on this [kaggle](https://www.kaggle.com/datasets/elmadafri/the-wildfire-dataset) page.

After that we fine tuned again the model on a very small secret dataset (provided by the use case partner) which contained images really close to the one received from real drones.
We did that since the first dataset was really big but the images were too diverse.

## Side Note
By inspecting the notebook you will see that the accuracy on validation is really low but it is fine. We overfitted on purpose the second dataset in order to have a model able to correctly predict the kind of images received by drones in a real scenario.
