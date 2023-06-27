# howto-.env-vite

## Description

This is a step by step guide on how to use enviroment variables in a Vite created React App. 

### Step 1: Install ```dotenv``` package.

In your terminal, install the ```dotenv``` package by entering ```npm install dotenv --save-dev```

<img src='https://github.com/vinceoct/howto-.env-vite/blob/main/assets/install.png' width='700' height='250'>

### Step 2: Import ```dotenv``` to your Vite config file.

A file called ```vite.config.js``` is created when you first create your app. To import ```dotenv```, open it and add the following line:
```import dotenv from 'dotenv'```
Then call ```dotenv.config()```.

<img src='https://github.com/vinceoct/howto-.env-vite/blob/main/assets/viteconfigjs.png' width='700' height='300'>

### Step 3: Create your ```.env``` file and define your environment variables. 

In your project's root directory, create a ```.env``` folder and define your environment variables. You must prefix them with ```VITE_``` in order for them to work. When making changes to your .env file you'll need to restart your server for the changes to take place. Don't forget to add your .env file to ```.gitignore``` before pushing to Github.    

<img src='https://github.com/vinceoct/howto-.env-vite/blob/main/assets/dotenvvariable.png' width='700' height='300'>

### Step 4: Access environment variables in your code. 

To access your newly created enviroment variables, use ```import.meta.env```.

<img src='https://github.com/vinceoct/howto-.env-vite/blob/main/assets/importmeta.png' width='700' height='175'>


