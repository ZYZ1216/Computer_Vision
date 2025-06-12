# Computer Vision Project

This project is the final project of computer vision. It is based on the Jetson-Nano platform and developed using the NVIDIA JetRacer ROS framework.
The final result is that the car can achieve autonomous path finding.

![image](https://github.com/user-attachments/assets/d93f23b6-1c36-4000-80b1-c8c8c373ab14)

## Main functions:
- [ ] Data sample collection and annotation platform based on Jupyter Notebook.
- [ ] Easy-to-use interactive platform for convolutional neural network training, solving lane perception through deep learning regression tasks.
- [ ] Use tensorRT forward network acceleration.
- [ ] Interactive console changes lanes through lane change buttons.
- [ ] Dynamic PD realizes corner closed-loop control.
- [ ] Straight/curved judgment and switching cruise speed.

## Instructions

### 1. Data collection
Run ``data_collection.ipynb``

The collected data is named target label + unique ID

Modify the number of target_names fields to change the number of perception lanes
Modify DATASET_DIR to change the data save address
### 2. Training model
Run ``trainData_model.ipynb``

Modify target_number to change the number of perception lanes
Modify epochs_widget to change the number of training iterations
Modify save_model_widget to change the model save address and name
### 3. Build inference acceleration engine
Run ``build_model.ipynb``

### 4. Lane cruising
Run ``inferenceControl.ipynb``
