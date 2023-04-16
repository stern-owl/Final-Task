# Final-Task
Task submission of Yash Aggarwal, 2022B1PS0930P

Here's the approach to the task:
 First, the program defines the parameters for the IMU data: the frequency at which the data will be generated (freq), the initial values for the accelerometer and gyroscope (accel_init and gyro_init, respectively).
 
 Next, the program defines the correction matrices for the accelerometer and gyroscope (accel_correction and gyro_correction, respectively). These matrices are used to correct for any biases.
 The program then initializes a ROS node and publisher for publishing the IMU data.
 
 The main loop of the program generates the accelerometer and gyroscope data by adding k values to the initial values. The program then applies the correction matrices to the sensor data to correct for any biases.

All the data gets published in the rostopic imu/data once the command rosrun is executed.

The data can further be processed using filters like EKF.
