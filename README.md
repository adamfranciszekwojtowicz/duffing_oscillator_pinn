# duffing_oscillator_pinn
In this project, a Physics Informed Neural Network is implemented to solve the Duffing oscillator problem. We combine ground truth with the Duffing equation to create a loss function, that lets the network learn efficiently. 
Input of the network is 8D: 5 oscillator parameters (alpha, beta, delta, gamma, omega) inital position x_0 and velocity v_0 and the time moment t. The output is 1D: position x in the input moment of time.
The training loop uses an autodifferention method to derive first and second derivatives for evaluating the equation.
Two accuracy metrics are used in this project: relative L2 error and tolerance based accuracy.