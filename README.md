# MachineLearning_Carprice_prediction_using_LinearRegression


# Problem Description

A Chinese automobile company aspires to enter the US market by setting up their
manufacturing unit there and producing cars locally to give competition to their US and
European counterparts. They have contracted an automobile consulting company to
understand the factors on which the pricing of cars depends. Specifically, they want to
understand the factors affecting the pricing of cars in the American market, since those may
be very different from the Chinese market. Essentially, the company wants to know:
• Which variables are significant in predicting the price of a car
• How well those variables describe the price of a car
Based on various market surveys, the consulting firm has gathered a large dataset of different
types of cars across the American market.

# Business Goal

You are required to model the price of cars with the available independent variables. It will be
used by the management to understand how exactly the prices vary with the independent
variables. They can accordingly manipulate the design of the cars, the business strategy etc. to
meet certain price levels. Further, the model will be a good way for the management to
understand the pricing dynamics of a new market.

##### Here's a brief overview of the columns in the dataset:

1. car_ID: Unique identifier for each car.
2. symboling: A rating that represents the risk level of the car. It can be positive, negative, or zero.
3. CarName: The name of the car model or brand.
4. fueltype: The type of fuel used by the car (e.g., gas, diesel).
5. aspiration: The aspiration method of the engine (e.g., std for standard, turbo for turbocharged).
6. doornumber: The number of doors on the car (e.g., two, four).
7. carbody: The body type of the car (e.g., convertible, hatchback, sedan).
8. drivewheel: The type of wheel drive (e.g., rwd for rear-wheel drive, fwd for front-wheel drive, 4wd for four-wheel drive).
9. enginelocation: The location of the engine (e.g., front, rear).
10. wheelbase: The distance between the front and rear axles of the car.
11. (ellipsis): Indicates that there are more columns in the dataset not shown in this excerpt.
12. enginesize: The size of the car's engine in cubic centimeters (cc).
13.fuelsystem: The type of fuel delivery system used in the engine (e.g., mpfi, which stands for multi-point fuel injection).
14. boreratio: The ratio of the cylinder bore diameter to stroke length.
15. stroke: The length of the piston stroke in the engine in millimeters.
16. compressionratio: The compression ratio of the engine.
17. horsepower: The engine's horsepower rating.
18. peakrpm: The engine's peak revolutions per minute.
19. citympg: The car's fuel efficiency in miles per gallon (mpg) during city driving.
20. highwaympg: The car's fuel efficiency in miles per gallon (mpg) during highway driving.
21. price: The price of the car.

## Steps Performed:
1) #### Data Loading:
      Started by loading the car dataset from a CSV file. This dataset contains various features (independent variables) related to cars, such as "drivewheel," "wheelbase," "carlength," etc., and a target variable "price," which represents the price of the car.
   
3) #### Preprocessing:
      We preprocessed the data, which involved handling missing values and converting categorical variables into numerical representations (if needed). Proper data preprocessing ensures that the data is in a suitable format for building the regression model.
   
5) #### Feature Selection:
      From the dataset, we selected the features with positive and negative correlations with the target variable "price." These features were "drivewheel," "wheelbase," "carlength," "carwidth," "curbweight," "cylindernumber," "enginesize," "fuelsystem," "boreratio," and "horsepower" for positive correlation, and "citympg" and "highwaympg" for negative correlation.
   
7) #### Feature Scaling:
      Since the selected features had different scales, we applied Min-Max scaling to bring all the features to a similar scale between 0 and 1. Feature scaling helps prevent certain features from dominating the model due to their larger magnitudes.

8) #### Data Splitting:
      We split the dataset into training and testing sets. The training set (80% of the data) was used to train the linear regression model, and the testing set (20% of the data) was used to evaluate the model's performance on unseen data.

9) #### Linear Regression Model:
      We created a linear regression model using the scikit-learn library. Linear regression is a simple and interpretable model that aims to fit a linear relationship between the selected features and the target variable "price."

10) #### Model Training: 
      The linear regression model was trained on the training data using the fit method. During training, the model learned the coefficients (weights) for each feature, aiming to minimize the mean squared error between the predicted prices and the actual prices.

11) #### Model Evaluation:
      Evaluated the model's performance on the testing set using various metrics:
          * Mean Squared Error (MSE): The average squared difference between the predicted prices and the actual prices. A lower MSE indicates better model performance.
          * R-squared (R²) Score: The proportion of variance in the target variable that is explained by the model. A higher R² score indicates a better fit to the data.
          * Cross-Validation RMSE: The average root mean squared error obtained through cross-validation. It gives an estimate of the model's performance on unseen data.
