
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

f(θ<sub>0</sub>, θ<sub>1</sub>) outputs a number. For this problem, 

f is some arbitrary/unknown smooth function (not necessarily the cost function of linear regression, so f may have local optima).

Suppose we use gradient descent to try to minimize f(θ<sub>0</sub>, θ<sub>1</sub>) as a function of θ<sub>0</sub> and θ<sub>1</sub>. Which of the following statements are true? (Check all that apply.)

* Setting the learning rate α to be very small is not harmful, and can only speed up the convergence of gradient descent.

* No matter how θ<sub>0</sub> and θ<sub>1</sub> are initialized, so long as learning rate α is sufficiently small, we can safely expect gradient descent to converge to the same solution

* If θ<sub>0</sub> and θ<sub>1</sub> are initialized at the global minimum, then one iteration will not change their values.

* If the first few iterations of gradient descent cause f(θ<sub>0</sub>, θ<sub>1</sub>) to increase rather than decrease, then the most likely cause is that we have set the learning rate α to too large a value


Explanantion:
--------------

* Setting the learning rate α to be very small is not harmful, and can only speed up the convergence of gradient descent.

**This is not True**

**When the learning rate α is too small, the gradient descent will take too many tiny (downhill) steps and decrease f(θ<sub>0</sub>,θ<sub>1</sub>) a little bit towards the convergence, so setting the learning rate to be very small, won't cause gradient descent to converge fast, but instead converging will be too slow**

* No matter how θ<sub>0</sub> and θ<sub>1</sub> are initialized, so long as learning rate α is sufficiently small, we can safely expect gradient descent to converge to the same solution

**This is not True**

**Depending on the initial conditions of the parameters (θ<sub>0</sub> and θ<sub>1</sub>), gradient descent may end up at different local optima.**


* If θ<sub>0</sub> and θ<sub>1</sub> are initialized at the global minimum, then one iteration will not change their values.

**This is True**

**Initializing θ<sub>0</sub> and θ<sub>1</sub> at a global minimum causes the derivative (gradient/slope) to be zero while calculating the gradient descent, so gradient descent will not change the parameter values. In more details:**

**θ<sub>j</sub> := θ<sub>j</sub> - α (partial derivative of J(θ<sub>0</sub>, θ<sub>1</sub>))
and since the dervative is zero, the parameter θ<sub>j</sub> won't be changed**

* If the first few iterations of gradient descent cause f(θ<sub>0</sub>, θ<sub>1</sub>) to increase rather than decrease, then the most likely cause is that we have set the learning rate α to too large a value

**This is True**

**If learning rate α is small enough, then gradient descent will always take too many tiny downhill steps and decrease f(θ<sub>0</sub>,θ<sub>1</sub>) a little bit. If gradient descent instead increases the cost (objective) function, this means learning rate α is too large and gradient descent won't converge or diverge.**


Answer:
------

* **If θ<sub>0</sub> and θ<sub>1</sub> are initialized at the global minimum, then one iteration will not change their values.**

* **If the first few iterations of gradient descent cause f(θ<sub>0</sub>, θ<sub>1</sub>) to increase rather than decrease, then the most likely cause is that we have set the learning rate α to too large a value.**

------------------------------------------------------------------------------------------------

Question 5:
-----------

Suppose that for some linear regression problem (say, predicting housing prices as in the lecture), we have some training set, and for our training set we managed to find some θ<sub>0</sub>, θ<sub>1</sub> such that J(θ<sub>0</sub>, θ<sub>1</sub>)=0.

Which of the statements below must then be true? (Check all that apply.)

* For this to be true, we must have θ<sub>0</sub> = 0 and θ<sub>1</sub> = 0 so that h<sub>θ</sub>(x)=0

* Gradient descent is likely to get stuck at a local minimum and fail to find the global minimum.

* Our training set can be fit perfectly by a straight line, i.e., all of our training examples lie perfectly on some straight line.

* For this to be true, we must have y^(i)=0 for every value of i=1,2,…,m.


Explanantion:
--------------

* For this to be true, we must have θ<sub>0</sub> = 0 and θ<sub>1</sub> = 0 so that h<sub>θ</sub>(x)=0

**This is not True**

**If J(θ<sub>0</sub>, θ<sub>1</sub>)=0, it means that the stright line defined by the hypothesis function (y = θ<sub>0</sub> + θ<sub>1</sub>)x) perfectly fits for all of our training data examples. Such a case, it is not necessarily or there is no reasons to expect that the values of θ<sub>0</sub> and θ<sub>1</sub> that achieve (J(θ<sub>0</sub>, θ<sub>1</sub>)=0), are both 0. **

* Gradient descent is likely to get stuck at a local minimum and fail to find the global minimum.

**This is not True**

**Having J(θ<sub>0</sub>, θ<sub>1</sub>)=0 causes the straight line to fit perfectly in our training data-set/examples and does not cause the gradient descent to stuck in the local minimum.**


* Our training set can be fit perfectly by a straight line, i.e., all of our training examples lie perfectly on some straight line.

**This is True**

**If J(θ<sub>0</sub>, θ<sub>1</sub>)=0 is the cost function (i.e. squared error function). This function is the mean of squares of the difference between the predicted value using hypothesis function h<sub>θ</sub>(x) and the actual values y is zero. To this end, the linear regression fits perfectly by a straight line**


* For this to be true, we must have y^(i)=0 for every value of i=1,2,…,m.

**This is not True**

**If all of our training examples fit perfectly by a straight line, we will be able to find θ<sub>0</sub> and θ<sub>1</sub>) so that J(θ<sub>0</sub>, θ<sub>1</sub>)=0. So, it is not necessary at all that y^(i) for all our examples should be zero.**

Answer:
------

**Our training set can be fit perfectly by a straight line, i.e., all of our training examples lie perfectly on some straight line.**
