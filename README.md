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
