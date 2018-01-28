
Question 1:
-----------

Consider the problem of predicting how well a student does in her second year of college/university, given how well she did in her first year.

Specifically, let x be equal to the number of "A" grades (including A-. A and A+ grades) that a student receives in their first year of college (freshmen year). We would like to predict the value of y, which we define as the number of "A" grades they get in their second year (sophomore year).

Here each row is one training example. Recall that in linear regression, our hypothesis is h<sub>θ</sub>(x) = θ<sub>0</sub> + θ<sub>1</sub> x, and we use m to denote the number of training examples.

| X  | Y | 
|----|---| 
| 5  | 4 |
| 3  | 4 |  
| 0  | 1 |  
| 4  | 3 | 


For the training set given above (note that this training set may also be referenced in other questions in this quiz), what is the value of m? In the box below, please enter your answer (which should be a number between 0 and 10).


Explanantion:
--------------

m is the number of the training sets or training examples.

Answer:
------

**m=4**

------------------------------------------------------------------------------------------------

Question 2:
-----------

Consider the following training set of m=4 training examples:

| X  | Y | 
|----|---| 
| 1  |0.5|
| 2  | 1 |  
| 4  | 2 |  
| 0  | 0 | 

Consider the linear regression model h<sub>θ</sub>(x)= θ<sub>0</sub> + θ<sub>1</sub>x. What are the values of θ<sub>0</sub> and θ<sub>1</sub> that you would expect to obtain upon running gradient descent on this model? (Linear regression will be able to fit this data perfectly.)


* θ<sub>0</sub> = 1, θ<sub>1</sub> = 0.5

* θ<sub>0</sub> = 0, θ<sub>1</sub> = 0.5

* θ<sub>0</sub> = 1, θ<sub>1</sub> = 1

* θ<sub>0</sub> = 0.5, θ<sub>1</sub> = 0

* θ<sub>0</sub> = 0.5, θ<sub>1</sub>  = 0.5



Explanantion:
--------------
Given that the linear regression fits perfectly, then the cost function (i.e. squared error function) J(θ<sub>0</sub>, θ<sub>1</sub>)=0. This function is the mean of squares of the difference between the predicted value using hypothesis function h<sub>θ</sub>(x) and the actual values y. 


Given the linear regression hypothesis function h<sub>θ</sub>(x)=θ<sub>0</sub>+θ<sub>1</sub>x
Using any value of x and its corresponding y from the table, we can easily get the answer. For instance

x= 4, y =2   →  2 = θ<sub>0</sub> + 4 θ<sub>1</sub>  →  θ<sub>0</sub> = 2 - 4 θ<sub>1</sub>  → I

x= 1, y =0.5  → 0.5 = θ<sub>0</sub> + θ<sub>1</sub>   →  0.5 = 2 - 4 θ<sub>1</sub> + θ<sub>1</sub> → II


3 θ<sub>1</sub> = 2 - 0.5  → θ<sub>1</sub> = 1.5/3 = 0.5

From I → θ<sub>0</sub> = 2 - 4 x 0.5 = 0



Answer:
------

**θ<sub>0</sub> = 0, θ<sub>1</sub> = 0.5**

------------------------------------------------------------------------------------------------

Question 3:
-----------
Suppose we set θ<sub>0</sub> = −1, θ<sub>1</sub> = 2 in the linear regression hypothesis from Q1. What is h<sub>θ</sub>(6)?


Explanantion:
--------------

h<sub>θ</sub>(x) = θ<sub>0</sub> + θ<sub>1</sub>x

h<sub>θ</sub>(6) = -1 + 2 x 6 = 11

Answer:
------

**h<sub>θ</sub>(6) = 11**

------------------------------------------------------------------------------------------------

Question 4:
-----------
Let f be some function so that

f(θ<sub>0</sub>, θ<sub>1</sub>) outputs a number. For this problem, f is some arbitrary/unknown smooth function (not necessarily the cost function of linear regression, so f may have local optima).

Suppose we use gradient descent to try to minimize f(θ<sub>0</sub>, θ<sub>1</sub>) as a function of θ<sub>0</sub> and θ<sub>1</sub>. Which of the following statements are true? (Check all that apply.)

* Setting the learning rate to be very small is not harmful, and can only speed up the convergence of gradient descent.

* No matter how θ<sub>0</sub> and θ<sub>1</sub> are initialized, so long as learning rate \alpha is sufficiently small, we can safely expect gradient descent to converge to the same solution

* If θ<sub>0</sub> and θ<sub>1</sub> are initialized at the global minimum, then one iteration will not change their values.

* If the first few iterations of gradient descent cause f(θ<sub>0</sub>, θ<sub>1</sub>) to increase rather than decrease, then the most likely cause is that we have set the learning rate to too large a value






Explanantion:
--------------

Answer:
------


------------------------------------------------------------------------------------------------

![alt text][Q5]

[Q5]: https://github.com/YasminFathy/Coursera-Machine-Learning-AndrewNg/blob/master/Week1/screenshots/Quiz2_Q5.png


Explanantion:
--------------

