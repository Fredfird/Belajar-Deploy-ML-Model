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
    ![picture](https://github.com/Fredfird/Belajar-Deploy-ML-Model/blob/master/model.png)
2. Run app.py using ‘python app.py’ command to start Flask API
    ![picture](https://github.com/Fredfird/Belajar-Deploy-ML-Model/blob/master/run%20app.png)
    By default, flask will run on port 5000.
3. Navigate to URL http://localhost:5000; Enter valid numerical values in all 3 input boxes     and hit Predict.
    ![picture](https://github.com/Fredfird/Belajar-Deploy-ML-Model/blob/master/locallhost.png)
4. Send direct POST requests to FLask API using Python's inbuilt request module 
    Run python request.py command to send the request with some pre-population values
    ![picture](https://github.com/Fredfird/Belajar-Deploy-ML-Model/blob/master/run_request.png)
    
Hosting the flask app

flask app hosted on the localhost can’t be shared with others since it’s “local”. Host the script to a free python hosting website called pythonanywhere by following a few simple steps:
1. Sign in for pythonanywhere account.
2. Add a new web app\
    I Choose flask and python version 3.7. After creating the web app, we will get a URL that points to flask endpoint. By default,         [username].pythonanywhere.com. My URL: fredfird.pythonanywhere.com
3. Install dependencies
    this ML model using various external libraries such as sklearn, numpy, pandas etc. Install all of them in your pythonanywhere           environment. To do so, open a new bash console and install libraries using pip. Make sure to install libraries with pip using           the user option because we don’t get the superuser rights.
    
    pip install flask flask_cors jsonify numpy pandas
    ![picture](https://github.com/Fredfird/Belajar-Deploy-ML-Model/blob/master/install%20library.PNG)
4. Upload the files
    Inside the default folder — /mysite/ you need to upload your complete folder. You can do it either using the files page on the           website or using the bash console by using wget command to download your files.
    ![picture](https://github.com/Fredfird/Belajar-Deploy-ML-Model/blob/master/upload.png) 
5. Reload the web app
   endpoint will now act as an API to facilitate other applications.
   ![picture](https://github.com/Fredfird/Belajar-Deploy-ML-Model/blob/master/reload.png)
   ![picture](https://github.com/Fredfird/Belajar-Deploy-ML-Model/blob/master/postman.PNG)


       





