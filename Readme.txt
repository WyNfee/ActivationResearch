This is the a project file eavaluate different activation function of neurons

Architecture of testing neuron network (NN)
* 1 input layer, 400 neurons
* 1 hidden layer, 100 neurons
* 1 output layer, 10 neurons

This neuron network using K-means, to recognize the handwriting digist from a subset of NMSIT database, where contains 5000 cases, each digits image is 20 * 20 size. (this is why we have 400 neurons as input)

How to use:
* Using MatLab to run the code, code should be able run with Octave, not tested
* To setup the project, run "script_A_RunFirst_SystemSettings.m"
* Folder Structure
	*Data: contains all data, including prepared training data and created data
		To clarify here, the data will auto generate in base directory, most of these data are copied in in the directory
	*NN: contains cost and gradient computation for this specific neural network
	*Ultis: contains all tool features used by other scripts, including weight initialization and activation function, etc.
* Naming Rule:
	* prefix:
		script_: means this file is a script file
		function_: means this file is a function
		data_: data file
	* function:
		Utils: means this file contains Utils features
		Ref: deplicated, no use at all
		CostFunction: means script will Compute the Cost Function
		Activation_Cost_Comparison: Compare the activation performance
		BGD: Batch Gradient Descent Method
		SGD: Stochastic Gradient Descent Method
		CG: Conjuction Gradient Method ( a type of analytics gradient optimizer)
		CD: Common Gradient Method (without any gradient optimizer)
	* Activation Type:
		Elu: Exponential Linear Unit activation
		Leaky: Leaky Rectifier Linear Unit activation
		ReLu: Recifier Linear Unit activation
		Tanh: Tanh activation
		Simoid: Sigmoid activation/Sigmoid Classifier
		Softmax: Softmax classifier

	Sample 1:
		function_Ref_CostFunctionELu_Softmax_BGD:
			means this script is a function script, and will use Elu as activation, and softmax as classifier, using BGD method to compute the cost function to work with this neuron network
	Sample 2:
		script_Tanh_SoftMax_SGD_CD
			measn this script is a entry point script, using Tanh as activation and Softmax as classifier, using SGD method, and no optimizer used to construct a learning algorithm
		
* To plot and check the performance of different activations
	Simply run:
		script_Activation_Cost_Comparison.m
		script_Activation_Cost_Comparison_SGD.m

Please reachout wangyifei52199@sina.com if you have any question and suggestions
		
		
