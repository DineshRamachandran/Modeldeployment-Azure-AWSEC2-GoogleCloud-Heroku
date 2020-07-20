Salary prediction

Predicting the salary based on experience. Used Regression model since label is continous.

I used different type of cloud service provider for Deploying Model 

1. Microsoft Azure
2. Google Cloud 
3. AWS EC2 
4. Heroku

1). Microsoft Azure (IAAS)

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

2). AWS EC2 instance

Install

1. Ubuntu
2. putty & putty gen
3. winscp


login AWS EC2 instance
EC2 - virtual server in the cloud
	Launch instance -creating the cloud server - where we can deploy the model and get api

ubuntu - generate the .pem file
	.pem file used to create private key to intract with the cloud environment

puttygen - using .pem file generate ppk file (private key)  

winscp- use ppk and host info from ec2 to login
	transfer file from one envs to another envs

putty - use ppk and host info from ec2 to login
          connect ubuntu server
          /home/ubuntu
	
          install 
          pip3 install pandas
	pip3 install -r requirement.txt
	python3 app.py

select api+:8080 

http://ec2-18-223-109-195.us-east-2.compute.amazonaws.com:8080

3). Google cloud:
          gcloud is the main command line tool of google cloud sdk which allow us to manage resources on google cloud platform and perform various developer workflow tasks.
                   
          Install Gcloud sdk installer - it bring the code to the gcloud env
          Main files are
                    main_app.py - model creation file
                    app.yaml   - runtime: python37
                    requirement.txt
                    
          login to console.cloud.google.com
          create project in IAM & ADMIN - manage resources - create project
          cmd prompt -change to working location  
                    gcloud init
                    gcloud app deploy app.yaml
          
      

4). Heroku Environment (PAAS)

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
