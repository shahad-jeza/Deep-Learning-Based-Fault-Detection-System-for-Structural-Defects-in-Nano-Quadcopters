# Deep Learning-Based Fault Detection System for Structural Defects in Nano-Quadcopters

This repository contains the code and resources for our research project on developing a deep learning model to detect structural defects in nano-quadcopters, particularly the Crazyflie 2.1. The model aims to enhance the safety and performance of UAVs by identifying faults in real-time using advanced neural network techniques.



# Deep Learning-Based Fault Detection System for Structural Defects in Nano-Quadcopters

## Overview

This project, proposed for the KAUST Academy AI Summer Training 2024, focuses on developing a deep learning-based system to detect structural defects in nano-quadcopters. The increasing use of unmanned aerial vehicles (UAVs), particularly nano-quadcopters, in various industries necessitates reliable systems for ensuring their operational integrity and safety. Our solution aims to identify fault signatures in real-time to prevent potential failures and extend the lifespan of these UAVs.

## Problem Statement

Nano-quadcopters are widely used due to their small size and agility, but structural defects can lead to critical failures. Traditional inspection methods often fail to detect early signs of damage. This project aims to develop a neural network (NN) model to detect these defects efficiently, ensuring the safety and reliability of the UAVs.

![Nano-Quadcopter](/Users/rawanyasir/Downloads/E8_W1_near_M3_M4.jpg)

## Objectives

- **Develop a Neural Network Model:** Create a model specifically designed for detecting structural defects in nano-quadcopters.
- **Assess Impact:** Analyze how these defects affect the drones' performance.
- **Compare Machine Learning Methods:** Evaluate different machine learning models to find the most efficient for real-time implementation on UAVs.
- **Dimensionality Reduction:** Apply techniques to improve the efficiency and speed of the fault detection model without compromising accuracy.
- **Optimize for Real-Time Application:** Ensure the model is suitable for deployment directly on UAVs for continuous monitoring.

## Methodology

- **Dataset:** We used the CrazyPAD (Crazyflie Propeller Anomaly Data) dataset, collected using the Crazyflie 2.1 nano-quadrotor, which includes data on both controller and motor performance under various fault conditions.
- **Data Preprocessing:** Missing values were imputed, and categorical labels were encoded. Feature scaling was applied using StandardScaler and QuantileTransformer.
- **Feature Engineering:** We created new features such as the magnitude of the position vector, spherical coordinates, and direction cosines, among others, to enhance model accuracy.
- **Models Tested:** Baseline models including XGBoost, Random Forest, k-Nearest Neighbors, and LightGBM were evaluated, along with a proposed Deep Neural Network (DNN) model.
- **Experimental Setup:** Experiments were conducted on the Ibex computational cluster with an x86 64 CPU and NVIDIA A100 GPU.

## Results

The DNN model outperformed all other models, achieving the highest accuracy, precision, recall, and F1 scores at 99%. It also demonstrated the fastest inference time, making it ideal for real-time fault detection in UAVs.

## Conclusion

This project demonstrates the effectiveness of deep learning models, particularly DNNs, in detecting structural defects in nano-quadcopters. The DNN model is recommended for applications requiring both high accuracy and fast inference times. Future work could focus on optimizing these models further for even greater efficiency and exploring hybrid approaches.

## Contributors

- **Shahad Jeza Alamri** - [Shahad.jeza.alamri@gmail.com](mailto:Shahad.jeza.alamri@gmail.com)
- **Rema Yasir Albarakati** - [Rema.y.albarakati@gmail.com](mailto:Rema.y.albarakati@gmail.com)
- **Shatha Turki Alsaidy** - [shathaalsaidy@gmail.com](mailto:shathaalsaidy@gmail.com)
- **Rawan Yasser Albarakati** - [Rawan.y.albarakati@gmail.com](mailto:Rawan.y.albarakati@gmail.com)
- **Salha Nasser Alyami** - [salha.nasser.ds@gmail.com](mailto:salha.nasser.ds@gmail.com)

