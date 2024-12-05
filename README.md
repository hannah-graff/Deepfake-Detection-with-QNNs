# Deepfake-Detection-with-QNNs
Research from Data Science Capstone Class <br>
Advisor: Dr. Steven Fernandes

### Overview

Deepfakes–the artificial manipulation of videos–are an ever-increasing threat in our digital world. With the growing prevalence of AI in our society, deepfakes have been used maliciously to steal identities, bully users online, create fake pornographic content, disseminate fake news, and threaten global security. Previous research has successfully implemented various methods and metrics (e.g., the ABC metric and RL-based tecture patches) to attack deepfakes. Under the guidance of Dr. Steven Fernandes, I aim to implement a Quantum Convolutional Neural Network (QNN) to detect deepfakes.

### Objectives

- advance the study and implementation of quantum computing via Quanvolutional Neural Networks
- outpace the growth of AI deepfake creation with the abilities of deepfake detection
- enhance processing efficiency
- propose a viable option for combatting deepfake detection

### Flow Diagram

![Updated Flow Diagram](https://github.com/user-attachments/assets/652bf867-2616-466c-b588-bd7592bb0724)

### Requirements

Python 3.10; Pennlyane library (for quantum)

### Steps

1. Generate

First, we create fake videos using a real and a donor video using the commercial website deepfakesweb.com. See below for an illustration of one of the examples. The full videos are above.

![Original_Donor_Fake Videos](https://github.com/user-attachments/assets/f8610213-eaa0-40ba-a63b-42bbcad77de7)

2. Preprocess

Next, we define a random quantum circuit and convolve the input image with it (preprocessing). A random 100 frames are taken from the original and the fake video, colnvolved, and then split into training and validation data. Finally, we preprocess the test images using our quantum circuit.

![preprcoess](https://github.com/user-attachments/assets/bddce1f6-c872-4a10-aec9-15f9c6f25a58)

3. Visualize

An example of the images inputted and outputted are below.

![colvolved images](https://github.com/user-attachments/assets/9d7d0910-af82-493e-bebc-180e234e62d4)

4. CNN Model

Then, we build, train, and test the CNN model. The accuracy and loss are reported below.

Classical Model Test Loss: 6.0351 <br>
Classical Model Test Accuracy: 26.48%

5. QNN Model

Similarly, we build, train, and test a QNN model. The accuracy and loss are reported below, followed by plots.

QCNN Model Test Loss: 1.4812 <br>
QCNN Model Test Accuracy: 71.16%

![trainingloss](https://github.com/user-attachments/assets/1f16f4a6-e289-4cc1-aa25-e38550be64fd)

6. Compare

Finally, we compare the two models' accuracy. For the examples we have been using, the QNN model is more accurate than the CNN model (71% vs. 26%) with less loss (1.48 vs. 6.03).
