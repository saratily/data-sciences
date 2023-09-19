**Glossary of Notations - Introduction to Deep Learning**

**x** = Input vector for the Neural Network

x<sub>i</sub> = i<sup>th</sup> component of the input vector **x**

**w** = The vector containing the weights for all the components of the input vector **x**

w<sub>i</sub> = i<sup>th</sup> componenet of the weight vector **w**

**w<sup>T</sup>** = Transpose of the weight vector **w**

d = Total number of input features

b = The bias Term

∑ 푤 푥 = Weighted sum of all input features starting from 푗 = 1 to 푗 = 푑, where 푗 is the iterator

z = Output of each neuron, i.e., the sum of “weighted sum of inputs” and “the bias”

f(z) = Activation function applied on the vector z

θ = The weight array **w** concatenated with the bias term

F(**x**; Θ) = The output of the neural network when the input given is **x** and the weights are given by the vector θ

Sigmoid = This is an activation function which takes an input and gives an output lying within the range of 0 to 1

tanh = This is an activation function which takes an input and gives an output lying withing the range of -1 to 1

ReLu = This activation function also called Rectified Linear Unit takes an input and returns it as it is, if it’s positive, and returns zero if the input is negative

a<sub>j</sub> = Softmax Activation Function

L(data; θ) = Loss term, i.e., the difference between the output of the Neural Network and the actual target variable, when the Neural Networks received the particular **data** and had the particular set of weights, i.e., θ

∆ω = Small change in weights ω

$\frac{\partial L}{\partial ω<sub>ij</sub>}$ = Partial derivative of the loss with respect to the particular weight given by ω

y<sup>i</sup> = The actual value of the target variable for the i<sup>th</sup> data point

F(**x**<sup>i</sup> ; θ) = The predicted output for the i<sup>tℎ</sup> data point

ω<sup>t</sup><sub>ij</sub> = The value of weight ω at time = t

ω<sup>t+1</sup><sub>ij</sub> = The value of weight ω at time = t + 1

η = Learning rate for updating the weights

λ = Regularization coefficient

$\frac{λ}{2}$ ||θ||<sup>2</sup> = Regularization term for L2 regularization
