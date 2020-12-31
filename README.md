#Estimator Implementation using C++

The main goal of this project is to implement an estimator for the drone by also combining the Controls developed in the previous project (Scenario 1-5).

**Scenario 6: Sensor Noise **

This step is simple. The simulator will provide GPS and IMU measurements. We need to calculate the standard deviation for the sensors. This can be done by loading the txt files and using the np.std function to find the SD. 

![](/Images/A_star.png)

**Picture 2

**Scenario 7: Attitude Estimation**

The next part is to estimate the roll, pitch and yaw by first finding the derivatives using the following formula and then integrating it. 


The integration is done by multiplying the derivatives with dt. 


**Scenario 8: Prediction**

The PredictState method and RbgPrime need to adapted using the following equations. 


**Scenario 9: Magnetometer**

Again refering to the paper Estimation for Quadrotors, and using the equations in the UpdatefromMag method, we will implement the magnetometer. 


**Scenario 10 : GPS Update**

The GPS update is performed by updating the equation for GPS update from the same paper. 

