# Single Layer Perceptron

This is a single layer Perceptron used for linear classification. I made it for a homework problem, but it can be trained on most basic binary datasets. It is ONLY capable of classifying linear datasets, for example it will not correctly classify a XOR function. 

# How it works

## Screenshots

![DataSet](https://i.ibb.co/thJYrfM/linear.jpg)

This dataset is linear as you can see by the blue line, the classes have a direct point where they are seperated. 

Using this dataset i assigned:
Black circles = 0 
White Circle = 1 

And chose initial weights w1 and w2 and the bias to be 0(it can be anything random between 0 and 1) Then I used that to calculate the weighted sum with the formula X_1 * W_1+X_2 * W_2 + B. Then the weighted sum is passed through and activation function, i chose a binary activation where if: W_Sum > 0 ; Output = 1. If: W_sum < 0 ; Output = 0. Using the output we calculate the error by subtracting the intended output by the actual output. 

This error is then used to update the weights and bias using the formulas 
* W_1=W_1+n(E*X1)
* W_2=W_2+n(E*X2)
* B=B+n(E)

This updating continues until your happy or until the whole epoch reaches an error rate of 0. 