# Thesis

Tool Wear Prediction Using Deep Learning Techniques on High Precision Milling Processes!
Complete Document found at UFSC repository: https://repositorio.ufsc.br/handle/123456789/204770

## License

The sofware systems and  data collected during this thesis are properties of Fraunhofer IPT - all rights reserved. Therefore, no code will be shown. What will be shown here is the documents explecitly allowed to be in public domain, including the thesis itself.
So, this repo aims to provide a brief resume about the activities developed during the Bachelor thesis, show pictures and results.

## Overview

The project is aimed to implement a system for tool wear prediction for high precision milling process. The approach chosen uses sensor data gathered from real test performed in a CNC machine center for precision milling combined with microscope measurement of tool flank wear. The acquisition software system implemented records data coming from: the spindle power consumption, acoustic and ultra-sonic emission, forces applied in the tool tip and vibration of the spindle body. Therefore, the project englobes the hardware and software setup for the acquisition system on the machine, process parameters planning and analysis of the data collected. The document discuss the use of different neural network architectures, feature extraction and training optimization techniques. For the project, three different deep-learning architectures were chosen for the prediction task (classification and regression were tested). The project compares the performance between each architecture and each used signal. The results showed a superior performance for the vibration data in combination with LSTMs which achieving 81% accuracy on classification and 176 μm  mean-squared-error on regression. The figure bellow abstract the overview steps of the project:

![alt text](https://github.com/eng-Marcio/Thesis/blob/master/Mysc/overview.PNG?raw=true)

the complete document can be found at UFSC repository: https://repositorio.ufsc.br/handle/123456789/204770

the thesis is divided into the following chapters:

1. Introduction: Describes the problem, the structure of the text in details and the solution approach.

2. State of The Art: Provides information about the literature solutions regarding  tool wear study and deep learning techniques.

3. Hardware Setup: Explain the equipment used, sensor instrumentation and the data acquisition devices employed on the experiments in order to gather the data. Besides that, it also informs the CNC configuration applied.

![alt text](https://github.com/eng-Marcio/Thesis/blob/master/Mysc/hardware_setup.PNG?raw=true)

4. Acquisition System Programming: Talks about Tama Client, a software solution for real time high frequency (up to 5 MHz) data acquistion. In order to fullfill the software requirements, a software project was developed. The system connects to Trialink Ring network (https://www.triamec.com/de/TAM-SDK.html) gather information comming from multiple devices and store all of it on local HDF files. Stored data went up to 5MBps including monitoring, GUI updates, integrity checking and compresssion. The software project is explained in details on the document.

![alt text](https://github.com/eng-Marcio/Thesis/blob/master/Mysc/TamaClientCD.png?raw=true)

5. Data Preprocessing: Explains the microscope measurements and the codes implemented in python using mainly Numpy to pre-process the data further used to train the networks. :snake:

![alt text](https://github.com/eng-Marcio/Thesis/blob/master/Mysc/vbs_tool4.png?raw=true)

6. Prediction Models: explains the algorithms, and codes used in order to train the models to infer the tool condition by observing sensor data inputs. Multiple different architectures were tested, and a new algorithm for Augmentation was proposed. At the end of this chapter, the accuracy of the networks obtained are provided.

![alt text](https://github.com/eng-Marcio/Thesis/blob/master/Mysc/results.PNG?raw=true)


## Notes

If you are an enthusiastic about data science or deep-learning applied to engineering problems, I deeply believe this thesis can help you to combine those tools with instrumentation and data acquisition, no matter which type of process you do want to study using AI. Much is speculated about the power of Industry 4.0 but we see little concrete results of its usage. I believe this work provides a concrete "how to" guide about measuring, storing, and using data on your shop-floor to do things which were not possible before the I4.0 era. If you seek for developping skills on this industry, I hope this work can be useful. Contact me if you have any feedback. :smile:

If you are a recruiter, I believe this document is the widest compilation of skills on engineering projects that I can provide by now (2020). :fire:
I know the thesis is quite long :sweat_smile:, but the chapters are very modular (yes, I praise a lot for modularity and scalability) so you can go directly to the chapter you are really interested in.

Have fun! :sunglasses:
