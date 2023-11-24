# Predicting Degradation Timelines of Commercial Turbofan Engines

Asset degradation in this context refers to the deterioration or decline in the condition of the components and subsystems that make up the propulsion system of an aircraft. The propulsion system of most high-speed airliners, such as commercial airplanes and fighter jets, are turbofan engines because they offer high thrust and fuel efficiency. NASA’s Prognostics Center of Excellence has developed sets of realistic turbofan data using a Matlab/Simulink tool called the Commercial Modular Aero-Propulsion System Simulation (C-MAPSS). The objective of this project is to train a learning model using this data to be able to make predictions about the degradation timeline for a given turbofan engine. 

******************The data:****************** I will be using the data available at https://data.nasa.gov/Aerospace/CMAPSS-Jet-Engine-Simulated-Data/ff5v-kuh6, which contains measurements taken at certain points in time for different turbofan engines. The measurements include 3 operational settings and 26 sensor measurements at each point in time for the engine. There are four sets of data, each distinguished by a different combination of one of the two flight conditions and one of the two fault modes. Each dataset contains a training set and testing set, in which the engines are operating normally at the start of the time series but develop a fault at some later point. In the training set, the fault grows with each cycle until the system fails, but in the testing set, the time series ends prior to the failure. The objective of the model will be to accurately predict the number of remaining operational cycles left before engine failure. 

****************************************Recommended reading:****************************************

- A. Saxena, K. Goebel, D. Simon, and N. Eklund, ”Damage Propagation Modeling for Aircraft Engine Prognostics”
- X. Zhang, L. Xiao, and J. Kang, ”Degredation Prediction Model Based on a Neural Network with Dynamic Windows”
- CMAPSS Documentation
