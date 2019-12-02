# Belajar-Deploy-ML-Model
Belajar-Deploy-ML-Model

ML-Model-Flask-Deployment
This is a demo project to elaborate how Machine Learn Models are deployed on production using Flask API
Project Structure
This project has four major parts :
1. model.py - This contains code fot our Machine Learning model to predict employee salaries absed on trainign data in 'hiring.csv' file.
2. app.py - This contains Flask APIs that receives employee details through GUI or API calls, computes the precited value based on our model and returns it.
3. request.py - This uses requests module to call APIs already defined in app.py and dispalys the returned value.
4. templates - This folder contains the HTML template to allow user to enter employee detail and displays the predicted employee salary.

Step:
1. Create the machine learning model, run model.py
    This would create a serialized version of our model into a file model.pkl
2. Run app.py using ‘python app.py’ command to start Flask API
    By default, flask will run on port 5000.
3. Navigate to URL http://localhost:5000; Enter valid numerical values in all 3 input boxes     and hit Predict.
4. Send direct POST requests to FLask API using Python's inbuilt request module 
    Run python request.py command to send the request with some pre-population values.
    [alt tag](https://github.com/Fredfird/Belajar-Deploy-ML-Model/blob/master/postman.PNG)






