# deep-learning-notes-andrew-ng


Supervised Learning 

Structured data & Unstructured data

Structured data
1. Each of features size,bedrooms,price will be having meaning
2.House Prediction
3.Advertising 

Unstructured data
1.Images
2.Voice 
3.Text

Why Deep learning working well?

the graph Amount of data vs Performance 

Traditional Algorithm 
Given more data don't know what to do
Small NN Performance will improve
Medium NN performance better than small NN
large NN performance is best

Labeled data

switching from sigmoid function to relu function gradient descent makes much faster
idea -----.> code -------> experiments

Computations can be better

1.Neural Network & DL 
2.
3.
4.


1.1 Introduction 
1.2 Basics of Neural Ntwrks programming
1.3 One hidden layer Neural Ntwrks
1.4 Deep Neural Netwroks Build
------------------------------------------------------------------------------------------------------------------
Deep learning Day 2

! binary classification 

CNN image recognize cat or not output 0 or 1
ex pixel 64*64*3 (Red,Yellow,Blue) into input feature vector 

Notation 

(x,y)    y belongs 0,1
(x1 , y1), (x2 , y2), (x3 , y3)

m training examples 
m test examples


x = [x1 ,x2, x3---------]  # stack into columns

nx , m shape of x

y = [y1, y2, y3-----]

1,m shape of y

x = input matrix
y = output matrix

Logistic Regression 


given X, want y hat = P(y=1/X)  0<y<=1

parameters w,b

output y hat =sigmoid (w transpose X+b)

sigmoid(z) = 1/1+e^-z

z = large sigmoid(z) -----  1
z = very small or very large negative number sigmoid (z)---- 0 

job learn w,b 

this is done by cost function 

in logistic regression mean square error will not be calculated generally

L(yhat,y) = 1/2(yhat- y)^2
L(yhat,y) = -(y*log(yhat)  + (1-y)log(1-yhat))

y = 1 ------    -log(yhat) want yhat =large
y = 0 ------    -log(1-yhat) want yhat = small

cost function J(w,b) = 1/m sigma L(yhat (i) , y(i))
we need to figure out parameters w,b such that cost function is minimized and loss function is minimized such that yhat and y are same 

gradient descent 

w = w - alpha(slope of  J(w,b))
b = b - alpha(slope of J(w,b))

---> alpha controls the steps of gradient descent to converge the function to zero.


Derivatives of calculus :
-------------------------
whatever is the value of a f(a) increases by 3 times
height to width ratio is 3:1 always 

f(a) = a^2
a = 2 , f(a) = 4
a = 2.0001 , f(a) = 4.004 
slope at a=2 is 4  

Computational graph 

J(a,b,c) = 3*(a + b*c)

u = b*c
v = a + u
J = 3*v

a = 5, b=3, c=2     ----- J = 33

Computing Derivatives
fix the value of u and change a 

Computational Graph helps in updating weights and bias through backward propagation steps.

1.


