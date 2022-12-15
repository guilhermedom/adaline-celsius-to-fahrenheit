# Adaline Converting Celsius to Fahrenheit

Adaline regressor learning the Celsius to Fahrenheit formula.

---

## Problem Overview

Temperatures are measured using 3 main metrics: Celsius, Fahrenheit and Kelvin. Each one of them can be obtained from any other using a linear function. The [Celsius to Fahrenheit conversion formula], for instance, is as follows:

$$ Fahrenheit = 1.8 * Celsius + 32 $$

Since it is a very simple formula, many machine learning algorithms are able to learn it and predict the conversion given a value in Celsius. Algorithms that have to fit coefficients for a weighted function can be interpreted intuitively in this task. The fitted coefficients, in this case, must be 1.8 for the single variable and 32 for the bias (or intercept).

We have a very simple dataset with only 30 instances and 2 variables. The independent variable is composed of random degrees Celsius. The dependent variable was built by calculating the corresponding degrees Fahrenheit for each instance. As this task is rather simple, this small dataset has more than enough data for a good model to learn the Celsius to Fahrenheit formula. Our data points are plotted in the next figure. The linear correlation between Celsius and Fahrenheit degrees is visible as the two variables plotted against each other form a line.

![adaline_celsius_to_fahrenheit_correlation](https://user-images.githubusercontent.com/33037020/207746212-895ece38-3ec8-4e9f-9b8c-2290657508c5.PNG)

## Analysis Introduction

Out of the many possible algorithm choices for building a model for this task, an [Adaline regressor] was the chosen one. Adaline is a neural network composed of a single neuron in a single layer, with no activation function. Adaline is a close variation of the [Perceptron], with the only difference being the lack of an activation function. This leads to Adaline models being fit using the output of the neuron directly instead of the output of the activation function for the neuron.

A simple regressor model like Adaline is applicable on this task given its simplicity. Since we have such a simple model, we can easily interpret it while maintaining a great performance.

In our tests, the Adaline regressor was able to correctly learn the conversion formula of degrees Celsius to degrees Fahrenheit. The next figure illustrates how the regression line perfectly intersects with all data points from our dataset.

![adaline_celsius_to_fahrenheit_regressor](https://user-images.githubusercontent.com/33037020/207746202-54470da7-0861-4565-84c1-ca8b92209ee2.PNG)

[//]: #

[Adaline regressor]: <http://rasbt.github.io/mlxtend/user_guide/classifier/Adaline/>
[Celsius to Fahrenheit conversion formula]: <https://www.thoughtco.com/chemistry-temperature-conversion-table-4012466>
[Perceptron]: <https://en.wikipedia.org/wiki/Perceptron>
