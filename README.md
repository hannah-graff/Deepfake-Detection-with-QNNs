# Deepfake-Detection-with-QNNs
Research from Data Science Capstone Class.

Advisor: Dr. Steven Fernandes

### Overview

Deepfakes–the artificial manipulation of videos–are an ever-emerging threat in our digital world. With the growing prevalence of AI in our society, deepfakes have been used maliciously to steal identities, bully users online, create fake pornographic content, disseminate fake news, and threaten global security. Previous research has successfully implemented various methods and metrics (e.g., the ABC metric, RL-based tecture patches) to attack deepfakes. Alongside Dr. Fernandes, I aim to implement a Quantum Convolutional Neural Network (QNN) to detect deepfakes.

### Objectives

- advance the study and implementation of quantum computing via Quanvolutional Nueral Networks
- parallel the advacements of deepfake detection with the advancement of AI and deepfake creation
- enhance processing efficiency
- propose a viable option for combatting deepfake detection

### Flow Diagram

![Flow Diagram (1)](https://github.com/user-attachments/assets/6a34ced0-05fd-4a12-a193-f384c0f735b8)

### Requirements

Python 3.10

### Steps

First, we create fake videos using a real and a donor video. See below for an illustration of one of the examples. The full videos are above.

![Original_Donor_Fake Videos](https://github.com/user-attachments/assets/f8610213-eaa0-40ba-a63b-42bbcad77de7)

Next, we preprocess the quantum circuit.

![preprcoess](https://github.com/user-attachments/assets/bddce1f6-c872-4a10-aec9-15f9c6f25a58)

After that, we visualize the images.

![input2](https://github.com/user-attachments/assets/beb1adeb-c061-458c-959d-310311e2e567)

Then, we build, train, and test the CNN model. A visualization of the accuracy and loss plots are outputted below.

![lossacc](https://github.com/user-attachments/assets/fbb2340c-136f-4569-ba5c-f4063b550ba6)

