# howto-.env-vite

## Description

This is a step by step guide on how to use enviroment variables in a Vite created React App. 

### Step 1: Install ```dotenv``` package.

Install the ```dotenv``` package by entering ```npm install dotenv --save-dev``` in your terminal.

<img src='https://github.com/vinceoct/howto-.env-vite/blob/main/assets/install.png' width='700' height='250'>

### Step 2: Import ```dotenv``` to your Vite config file.

A Vite config file called ```vite.config.js``` should already exist in your root directory by default. To import ```dotenv```, open ```vite.config.js``` and add the following lines:
```import dotenv from 'dotenv'```
```dotenv.config```.

<img src='https://github.com/vinceoct/howto-.env-vite/blob/main/assets/viteconfigjs.png' width='700' height='300'>

### Step 3: Create your ```.env``` file and define your environment variables. 

In your project's root directory, create a ```.env``` file and define your environment variables. You must prefix them with ```VITE_``` in order for them to work. When making changes to your ```.env``` file, make sure you restart your server. Otherwise, the changes won't take place. In the following example, we're defining enviroment variables for an API Key and an email address.     

<img src='https://github.com/vinceoct/howto-.env-vite/blob/main/assets/dotenvvariable.png' width='700' height='300'>

*Don't forget to add ```.env``` to your ```.gitignore``` file before pushing to Github.* 


### Step 4: Access environment variables in your code. 

To access your newly created enviroment variables, use ```import.meta.env```. In this example, we're accessing ```VITE_EMAIL``` using ```import.meta.env.VITE_EMAIL```

<img src='https://github.com/vinceoct/howto-.env-vite/blob/main/assets/importmeta.png' width='700' height='175'>


