# Harmonic Monitoring and Suppression System for Distributed Smart Grid in Public Buildings

------

This project mainly implements SDAFS(Spatial Distributed Active Filter System) in large public buildings, and provides corresponding solutions considering  smart grid (SG) and smart buildings for better Human-computer interaction and IoT transmission stability.The projects completed by our team are as follows:

> *  [Architectural modeling based on SketchUp®](https://github.com/Jason-Cooperate/Harmonic-Monitoring-and-Suppression-system-for-Distributed-Smart-Grid-in-Public-Buildings/tree/master/Architectural%20modeling)
> *  [Distribution topology of APF in public buildings based on MATLAB® & EnergyPLUS®](https://github.com/Jason-Cooperate/Harmonic-Monitoring-and-Suppression-system-for-Distributed-Smart-Grid-in-Public-Buildings/tree/master/Building%20Simulation)
> *  [LCLCL Active Power Filter Subsystem construnction](https://github.com/Jason-Cooperate/Harmonic-Monitoring-and-Suppression-system-for-Distributed-Smart-Grid-in-Public-Buildings/tree/master/DAFS)
> *  [Smart grid monitoring based on RTSG algorithm and Artificial Neural Network](https://github.com/Jason-Cooperate/Harmonic-Monitoring-and-Suppression-system-for-Distributed-Smart-Grid-in-Public-Buildings/tree/master/RTSG%20algorithm%20and%20ANN)

Summary diagram of this project:
![SDAFS Strructure](https://github.com/Jason-Cooperate/Harmonic-Monitoring-and-Suppression-system-for-Distributed-Smart-Grid-in-Public-Buildings/blob/master/Picture/总图2.jpg)

## 1. Architectural modeling
  We modeled a large public building in Shanghai to provide a simulation basis for EnergyPlus.
 [details](https://github.com/Jason-Cooperate/Harmonic-Monitoring-and-Suppression-system-for-Distributed-Smart-Grid-in-Public-Buildings/tree/master/Architectural%20modeling)

## 2. Building Consumption simulation
  We set up the parameters in E+ and run the model to obtaion the results.
 [details](https://github.com/Jason-Cooperate/Harmonic-Monitoring-and-Suppression-system-for-Distributed-Smart-Grid-in-Public-Buildings/tree/master/Building%20Simulation)

## 3. LCLCL Active Power Filter Subsystem construnction
  We made a single initial generation LCLCL active filter subsystem through simulation based on matlab and PCB production based on Aultim Designer, and then programmed in the CSS9.0 environment.
 [details](https://github.com/Jason-Cooperate/Harmonic-Monitoring-and-Suppression-system-for-Distributed-Smart-Grid-in-Public-Buildings/tree/master/DAFS)

## 4. Smart grid monitoring based on RTSG algorithm and Artificial Neural Network
  We proposed the RTSG (Real Time Synchronized Goertzel) algorithm and conducted simulation tests on MATLAB. In addition, we also quoted the CNN in the paper<sup>[1]</sup> and processed the MCT vectors to obtain the classification results of power quality disturbances.
  [details](https://github.com/Jason-Cooperate/Harmonic-Monitoring-and-Suppression-system-for-Distributed-Smart-Grid-in-Public-Buildings/tree/master/RTSG%20algorithm%20and%20ANN)

## 5. REFERENCE

  - [1] Ma J , Zhang J , Xiao L , et al. Classification of Power Quality Disturbances via Deep Learning[J]. IETE Technical Review, 2016:1-8.

------

     [Unable to load Pictures?](https://zhuanlan.zhihu.com/p/107196957)

------

       Author [@Jasonmils][2]     
       4.3  2020

------
[2]:https://github.com/Jasonmils
