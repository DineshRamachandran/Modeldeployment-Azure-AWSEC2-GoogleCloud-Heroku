Salary prediction

Predicting the salary based on experience. Used Regression model since label is continous.

I used different type of cloud service provider for Deploying Model 

1. Microsoft Azure
2. Google Cloud 
3. AWS EC2 
4. Heroku


1. Microsoft Azure (IAAS)

CI / CD - continous integration & continous deployment process
Developer need to takecare:  Application / Data 
Service provide takecare : runtime / os / storage / service / networking

Step1: Create Resource - web app - provide necessary info
          Resource group
          name
          runtime stack
          region
Step2: Development center 
          select anyone - github / Azure repos / bitbucket 
          App service Build service
          once deployment completed copy url overview page
 
 https://aqijaiput.azurewebsites.net


2. Heroku Environment (PAAS)

Platform as a service:
Developer need to takecare:  Application / Data 
Service provide takecare : runtime / os / storage / service / networking

Step for Deploying ML Model

1. Train the model
2. Create web app using flask
3. Upload the code in github
4. create an application in HEROKU(PAAS)
5. Link the github to Heroku application
6. Deploy the model manually in Heroku app
7. Global web app is ready

https://salpredictions.herokuapp.com/
