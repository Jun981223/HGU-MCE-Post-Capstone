Simulation and Experimental Data Description
This project applies surrogate modeling using two types of data sources: simulation and experiment. The structure and usage for each is described below.


1. Simulation-based Data
The full simulation process is implemented in the MATLAB script:
FINAL.m

Running FINAL.m will:
Generate sample suspension parameter sets
Run dynamic simulations
Extract response features such as roll angle, pitch rate, and heave acceleration
Save the results for use in surrogate modeling


2. Experiment-based Data
Experimental data consists of 20 CSV files collected from IMU sensors during real vehicle tests.
Each file corresponds to one test case, and is named as:
experiment_data/
├── imu1.csv
├── imu2.csv
├── ...
└── imu20.csv


MATLAB scripts for processing experimental data are provided in the experiment_code/ directory. Each script is dedicated to analyzing a specific dynamic feature (e.g., pitch, roll, heave).

📌 Important:
The experiment_data/ folder must be placed in the same directory where the experimental MATLAB scripts are executed. Otherwise, the scripts will not be able to load the data correctly.
