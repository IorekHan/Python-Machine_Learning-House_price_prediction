# House Price Prediction
### 6893-project

This is a course project of Columbia University 6893 course in 2022 fall semester. This project is done by: Linyang Han, Ke Li and Chu Qin.

<br>

## Intro
This project use different Machine Learning models to apply prediction on house price in the US. 
<br>
Used datasets are saved in /datasets.
The data set is already cleaned.
<br>
The front-end is based on React.
For acceptable waiting time for visualization, only NY and NJ data is applied to the front-end map.

## Run App
All our code for model training are stored inside `./model-code/`.

Run `./install.sh` to install all the dependent software like node and python.

To deploy the app:

1. Host Python back-end application with `nohup python3 predict.py` to run the app as a background process

2. Change ip address in UserForm.js file to the ip address of the hosting machine

3. Go to root directory of the front-end application with `cd front-end` 

4. Use npm to build the application into production with `npm run build`

5. Host React front-end application with `pm2 serve -- build` to run the app as a background process

6. Note: The demo model we choose is the random forest model `rf_model.pkl`, you can replace it with your own model and adjust the name of the model in predict.py accordingly
