# **Parameter Optimization of SVM**

This repository contains Python code for optimizing the parameters of a Support Vector Machine (SVM) classifier using Bayesian Optimization. The goal is to enhance the classification performance of the SVM algorithm.

## **Introduction**

Support Vector Machine (SVM) is a powerful supervised learning algorithm used for classification tasks. However, the performance of SVM heavily depends on the choice of its parameters, such as the kernel type, regularization parameter (nu), and tolerance (tol). This project focuses on optimizing these parameters to achieve higher accuracy in classification tasks.

## **Implementation**

The optimization process is implemented using Bayesian Optimization, leveraging the `bayesian-optimization` library. The dataset used for training and testing the SVM classifier is fetched from the UCIML repository. The code is organized into the following sections:

1. **Importing Libraries**: Necessary libraries including `numpy`, `pandas`, and `sklearn` are imported.
2. **Fetching and Organizing Dataset**: The dataset is fetched and organized into feature and target variables. It is then split into training and testing sets.
3. **Defining Optimization Parameter Ranges**: Ranges for the optimization parameters (kernel type, nu, tol) are defined.
4. **Function for Evaluating SVM**: A function is defined to evaluate SVM with given parameters, calculating accuracy using the test set.
5. **Bayesian Optimization for Multiple Samples**: Bayesian Optimization is performed for multiple samples, with results recorded including the best accuracy and corresponding SVM parameters.
6. **Visualization of Convergence Plots**: Convergence plots for each sample are visualized to demonstrate the optimization process.
7. **Creating DataFrame for Results**: Results including sample number, best accuracy, and corresponding SVM parameters are presented in a DataFrame.
8. **Finding Sample with Maximum Accuracy**: The sample with the maximum accuracy is identified from the results.
9. **Plotting Convergence for Maximum Accuracy Sample**: Convergence plot for the sample with the maximum accuracy is generated.

## **Usage**

To use this code:

1. Ensure you have Python installed on your system.
2. Install the required libraries using `pip install -r requirements.txt`.
3. Execute the Jupyter notebook `ParameterOptimizationofSVM.ipynb` in a compatible environment.

## **Conclusion**

This project demonstrates the importance of parameter optimization in improving the performance of machine learning algorithms, particularly Support Vector Machines. By leveraging Bayesian Optimization techniques, significant improvements in classification accuracy can be achieved. Feel free to explore and adapt the code to your specific datasets and classification tasks.
