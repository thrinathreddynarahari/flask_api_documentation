# Deploying a flask-application in Heroku

To deploy a application in Heroku which developed using flask use the following steps.

## Create a git repository

Create a public repository and add gitignore as python.
![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/assets/main/git-api.png)

## Step 1

## Create a python file in the same application folder by the name

```
wsgi.py
```

## Add the following code in the wsfi.py

```

from Synchro_API import app

if __name__ == '__main__':
    app.run()

```

## the code should look like this

![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/assets/main/flask_code_images.png)

## Step 2

## Create a text file in the same folder by name

```
runtime.txt
```

Add the following in the runtime.txt

```
python-3.9.6
```

## the code should look like this

![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/assets/main/runtime.png)

## Step 3

Create an another file by name **Procfile**

```
Procfile
```

Add the following content inside the **Procfile**

```
web: gunicorn  main:app
```

## Procfile should look like this

![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/assets/main/profilic.png)

## Step 4

## Open the python terminal and run the following command this will generate a **requriements.txt** file in the project directory which consists of the information of modules and packages that we have used in our application.

```
pip freeze > requirements.txt
```

## Inside the requriements.txt the generated code would look something like this

![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/assets/main/profilic2.png)

> **Clone this code to git Repository**

## Step 5

## Till now we have setup our project for deployment now we have to set Heroku.

Sign up for Heroku for using this link [Click Here ](https://signup.heroku.com/)

## Step 6

Create a new app by providing the name you want
![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/assets/main/profilic2.png)

## Step 7

Click on connect to git repository.
![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/assets/main/heroku_git_link.png)

Search the git repository which is created earlier.
![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/assets/main/heroku_git_account.png)

connect to your repository
![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/assets/main/heroku_git_connect.png)

## Step 8

Click on **"Enable Automatic Deploys"**
![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/assets/main/heroku_git_click_on_deploy.png)

Deploy the main branch
![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/assets/main/heroku_git_deploy_branch.png)

wait untill it deploys you application.

![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/assets/main/heroku_final.png)

**Done !**
**You have deployed a flask application on Heroku !**

You will get the host link after clicking on view now you can check your apis using this link using postman.
