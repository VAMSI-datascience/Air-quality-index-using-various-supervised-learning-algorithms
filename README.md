# Webapp for Air quality index using various supervised learning algorithms... 


[This is the website where we are web scrapping the real time data for our quality index prediction](https://en.tutiempo.net/)

## This is a special project because it is not done on regualr datasets which are available to everyone, but we extracting our own data using web scrapping tools and we are using that real time data to predict the quality index..

![climate](https://user-images.githubusercontent.com/51853466/82449727-4bdb7900-9ac9-11ea-9d98-c2566b3f4dfd.PNG)

+ The above picture the website from which where we are extracting the data from..

![climate2](https://user-images.githubusercontent.com/51853466/82449807-67468400-9ac9-11ea-8c39-a37c317b172b.PNG)

+ The above represents the data descrition that we are working on and gives the insight of the data set which we are extracting..

+  **Firstly**, the dataset comprises of data from 2 websites, one is from the above mentioned another is from the paid thirdparty api..
+  The data we are using is from 2013 to 2019 that is the pm2.5 value and we are downloading this data from third party api and it is paid one and there is a folder called AQI in our repository where the data collected can be seen..

+ In the **second** part of our data collection, as we can see that the pm2.5 values are given in a hourly basis and the data we are extracting is in daily basis.. The target for us is we need to find the avg value of the pm2.5 for 24 hours and make it as its daily value.. And that part can be seen in the **plot_aqi.py** file in the repo..

+ In the **third** part what we are doing is we are a tool called **Beautifulsoup** in order the extract the information we need from the website and finally we are combining our both the datasets and forming it as independent and the dependent features and combining to form a single dataset for our model prediction..And that part is shown in the **combine.py** file..

+ And finally we are training our dataset and applying the best algorithm in order to get the better accuracy..we are training the following models..

**1 Randomforest model**

**2 Knearest neighbours**

**3 Decision tress**

**4 Xgboost classifier**

+ For each and every alogorithm, exploratory data analysis has been performed and is mentioned with their respective **.pynb** notebooks..

+ And out of all the classifiers **Randomforest classifier** outperformed all the other models in terms of accuracy and MAE, MSE, RMSE etc..and we have saved it as **pickle** file for our model deployment..

## Regression Evaluation Metrics

![brgijb](https://user-images.githubusercontent.com/51853466/82566643-d8ee0300-9b99-11ea-8092-89d268a30e10.PNG)

+ And finally we have used **Flask Framework** for deploying it in the cloud platforms.. and we have used **Heroku** cloud platform for deploying the web application and this is executed by the **app.py** file and the **requirements.txt** and the **procfile** has been mentioned as web application..

[Click here to View the sample web app prediction of bangalore and click predict](https://airqualityindexpred.herokuapp.com/)- **DISCLAIMER** Link undergoing some issues try below steps.

## How to run the project?

1. Install all the libraries mentioned in the [requirements.txt]
2. Clone this repository in your local system.
3. Open the command prompt from your project directory and run the command `app.py`.
4. Go to your browser and type `http://127.0.0.1:5000/` in the address bar.
5. Hurray! That's it.

![jyty](https://user-images.githubusercontent.com/51853466/82567386-ebb50780-9b9a-11ea-9863-6836b8302be9.PNG)

+ This is how a webapp prediction looks like... 





