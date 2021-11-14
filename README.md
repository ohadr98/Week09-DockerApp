
# Docker    <img src="https://www.docker.com/sites/default/files/d8/styles/role_icon/public/2019-07/horizontal-logo-monochromatic-white.png?itok=SBlK2TGU" width="400" height="130" align="right"/>

In this project we were asked to create 2 environment - staging/production
and create CICD with Docker 

## Requirements and Installations:
- [Node.js](https://nodejs.org/) 12.x or higher

- [Free Okta developer account](https://developer.okta.com/) for account
  registration, login

- Install Docker on your VM by :`sudo apt-get upadte && sudo apt install docker.io`

## Instructions
- Create a Dockerfile for the app and add it to repository
 
- Configure your pipelines using Yaml pipelines that uses different stages to separate the processes.
  Your Yaml need to consists from: CI, CD staging and CD production
  
- Enter to One Of your machine and create agent using  [System prerequisites](https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/v2-windows?view=azure-devops#check-prerequisites)

- You need to create Environments in azure devop for staging and production  and add the Prod VM to the Production and staging VM to Staging (Environment support the Yaml and     deployment group are not

- To get docker permissions you need to write in each machine `sudo chmod 777 /var/run/docker.sock`

- You need to create Environment Varibles in azure pipeline for all the secret varibles

- When you finish to add all the varibles run the pipeline and run in the broswer your hosturl:8080 to see if the app running
  




# Node.js Weight Tracker:

![build-weight-tracker-app-demo](https://user-images.githubusercontent.com/83014719/137505630-ccf4c3f4-6e06-4778-b414-830d6bb23f99.gif)
This sample application demonstrates the following technologies.
- [hapi](https://hapi.dev) - a wonderful Node.js application framework
- [PostgreSQL](https://www.postgresql.org/) - a popular relational database
- [Postgres](https://github.com/porsager/postgres) - a new PostgreSQL client for Node.js
- [Vue.js](https://vuejs.org/) - a popular front-end library
- [Bulma](https://bulma.io/) - a great CSS framework based on Flexbox
- [EJS](https://ejs.co/) - a great template library for server-side HTML templates

## Install and Configuration
1. Clone or download source files
1. Run `npm install` to install dependencies
1. If you don't already have PostgreSQL, set up using Docker
1. Create a [free Okta developer account](https://developer.okta.com/) and add a web application for this app
1. Copy `.env.sample` to `.env` and change the `OKTA_*` values to your application
1. Initialize the PostgreSQL database by running `npm run initdb`
1. Run `npm run dev` to start Node.js
