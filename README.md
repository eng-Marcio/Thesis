# Thesis

Tool Wear Prediction Using Deep Learning Techniques on High Precision Milling Processes!

## License

The sofware systems and  data collected during this thesis are properties of Fraunhofer IPT - all rights reserved. Therefore, no code will be shown. What will be shown here is the documents explecitly allowed to be in public domain, including the thesis itself.
So, this repo aims to provide a brief resume about the activities developed during the Bachelor thesis, show pictures and results.

## Overview

The project is aimed to implement a system for tool wear prediction for high precision milling process. The approach chosen uses sensor data gathered from real test performed in a CNC machine center for precision milling combined with microscope measurement of tool flank wear. The acquisition software system implemented records data coming from: the spindle power consumption, acoustic and ultra-sonic emission, forces applied in the tool tip and vibration of the spindle body. Therefore, the project englobes the hardware and software setup for the acquisition system on the machine, process parameters planning and analysis of the data collected. The document discuss the use of different neural network architectures, feature extraction and training optimization techniques. For the project, three different deep-learning architectures were chosen for the prediction task (classification and regression were tested). The project compares the performance between each architecture and each used signal. The results showed a superior performance for the vibration data in combination with LSTMs which achieving 81% accuracy on classification and 176 μm  mean-squared-error on regression. The figure bellow abstract the overview steps of the project:

![alt text](https://github.com/eng-Marcio/Thesis/blob/master/Mysc/overview.PNG?raw=true)
