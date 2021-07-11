# Prediction of Surface Temperature in Continuous Casting of Steel Using Artificial Neural Networks
This project includes the supplementary python code for my Bachelor's thesis about the predicition of the surface temperature in the continouus casting of stell using artificial networks such as Multilayer Perceptrons (MLPs) and Long Short Term Memory networks (LSTMs). The following Abstract provides an overview of the thesis.

# Abstract 
This thesis presents an approach to use Artificial Neural Networks to model the process of continuous casting of steel in order to predict the surface temperature the steel strand.
        
In the continuous caster at hand the steel strand is bent by 90 degrees before leaving the machine. During bending, the surface temperature of the strand plays an important role for the quality of the steel. Typically, a physical temperature model, using a non-linear PDE, is used to model the temperature of the steel strand as it's processed in the continuous caster. The temperature model is very sensitive to the right choice of free parameters. Those have to be adapted to real situation of the plant repeatedly and at great expense.

This work aims to explore the potential and limitations of using data-based models to model the temperature in the caster.

We conduct and present a thorough analysis of the different parameter that are involved in the steel casting process, before we evaluate two different, suitable types of deep learning models.

We train and evaluate a large range of configurations of MLPs and LSTMs models. 
Both models are able to model the process on an held out test set reasonably well. However we find that in the stable phase of the process both miss to model fluctuations and tend to predict a constant value close to the mean for that area.
Comparing the best configuration of each of those types of models, we find that the LSTM slightly outperforms the MLP in predicting on an held out test set.

In a sensitivity analysis we find, as expected, that the model can only perform well on data that is within reasonable range of the data collected in the process and does not model the underlying physical and causal dependencies outside of that range well.

Therefore, it is not advisable to perform inverse modeling - i.e. using the model to find parameter values that would lead to a desired temperature under the model in a real world setting.

# Data
This work was done in cooperation with a leading European steel producer and the data used are actual production data. Due to legal reasons, these data cannot be provided.

# Authors
- Enrico Eisen
