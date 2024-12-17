# Turbine Energy Yield Prediction for Gas Turbine Optimization
This project uses machine learning to predict Turbine Energy Yield (TEY) from gas turbine data. The goal is to identify operational conditions and turbine settings that maximize energy output, ensuring the power plant operates at its highest efficiency and reducing fuel consumption and operational costs. 

## Dataset Attribution
The dataset used in this project is from the Gas Turbine CO and NOx Emission Data Set available at the UCI Machine Learning Repository. The data was collected from a gas turbine in Turkey's northwestern region, focusing on emissions and operational conditions.


**Source:** UCI Machine Learning Repository. (2019, November 28). Gas Turbine CO and NOx Emission Data Set.

[Dataset Link](https://archive.ics.uci.edu/dataset/551/gas+turbine+co+and+nox+emission+data+set)

**Key Objectives:**

* **Predict TEY:** Accurately forecast turbine energy yield based on sensor data.
* **Optimize Operations:** Identify optimal turbine settings and operational conditions for maximum energy output.
* **Reduce Costs:** Minimize fuel consumption and operational expenses by improving efficiency.
* **Predictive Maintenance:** Identify potential issues like turbine component degradation by detecting deviations from normal operating conditions.

## About The Dataset

The dataset used in this project contains 36733 instances of 11 sensor measures aggregated over one hour from a gas turbine located in Turkey's north western region. The data was collected between 2011 and 2015 and includes gas turbine parameters (such as Turbine Inlet Temperature and Compressor Discharge pressure) in addition to ambient variables. The data is chronologically sorted, and the first three years' data is used for training and cross-validation, while the last two years are used for testing.

**Dataset Source:** The dataset is publicly available and can be accessed through the UCI Machine Learning Repository.

**Features:**

The dataset includes the following features:

* Ambient temperature (AT)
* Ambient pressure (AP)
* Ambient humidity (AH)
* Air filter difference pressure (AFDP)
* Gas turbine exhaust pressure (GTEP)
* Turbine inlet temperature (TIT)
* Turbine after temperature (TAT)
* Compressor discharge pressure (CDP)
* Turbine energy yield (TEY) - **Target variable**
* Carbon monoxide (CO)
* Nitrogen oxides (NOx)

## Methodology

1. **Data Preprocessing:**
    * Handling missing data (if any)
    * Handling duplicates
    * Data transformation (handling skewness and outliers)
    * Feature scaling

2. **Feature Selection:**
    * Correlation analysis
    * SelectKBest method
    * Multicollinearity check and optimization

3. **Model Implementation:**
    * Linear Regression
    * Decision Tree Regressor
    * Random Forest Regressor
    * Gradient Boosting Regressor
    * Support Vector Regressor

4. **Model Evaluation:**
    * Mean Squared Error (MSE)
    * R-squared (R²)
    * Mean Absolute Error (MAE)

5. **Model Selection and Deployment:**
    * Linear Regression trained on the IQR outlier-capped dataset was selected as the best model.
    * The final model was saved using a pipeline, including preprocessing steps for seamless deployment.

## Results

The Linear Regression model achieved high accuracy in predicting Turbine Energy Yield (TEY), with:

* MSE: 4.56
* MAE: 1.78
* R²: 0.98

These results demonstrate the model's effectiveness in capturing the data variability and making accurate predictions.

## AMN Al Turbine Energy Yield Predictor App 
I am currently working on app development, where this model will come to life. This is a screenshot of the app in its development phase. Once completed, I will publish the app and provide all relevant details in a different repository. I will also update the README file here and add an app download button in the Downloads section below.
![git](https://github.com/user-attachments/assets/89cfdb91-3d9a-4bb7-9c48-4cb477bb00e3)


## Conclusion

This project successfully developed a machine learning model for predicting Turbine Energy Yield (TEY), offering valuable insights for optimizing gas turbine operations. The model can help power plant operators identify ideal turbine settings and operational conditions to maximize energy output, reduce costs, and implement predictive maintenance strategies.

## Limitations

* Data Specificity: The model was trained on data from a single power plant. Applying it to different power plants or regions may require retraining.
* Data Collection Period: The model was trained on data collected within a specific timeframe. Over time, turbine behavior can change, affecting model performance.

## Future Work

* Incorporating Additional Features: Include maintenance data, fuel quality, and other relevant parameters to improve model accuracy.
* Real-Time Predictive Maintenance: Develop models for predicting turbine degradation and integrate real-time sensor data for condition monitoring.
* Scalability and Generalization: Test the model across multiple power plants to assess its generalizability.
* Integration with Control Systems: Deploy the model in real-time systems for continuous monitoring and automated decision-making.


## Usage

1. Clone the repository
2. Install the required libraries
3. Run the Jupyter Notebook: `Turbine_Energy_Yield_Prediction_for_Gas_Turbine_Optimization.ipynb`
4. **Or, run the notebook in Google Colab:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aneeshmurali-n/ML-Turbine-Energy-Yield-Prediction-for-Gas-Turbine-Optimization/blob/main/Turbine_Energy_Yield_Prediction_for_Gas_Turbine_Optimization.ipynb)


## Downloads
[![Download](https://img.shields.io/badge/Download-Turbine_energy_yield_prediction_model-blue)](https://github.com/aneeshmurali-n/ML-Turbine-Energy-Yield-Prediction-for-Gas-Turbine-Optimization/raw/main/turbine_energy_yield_prediction_model_by_amn.zip)



