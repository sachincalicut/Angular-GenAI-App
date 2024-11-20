<div align="center">
  <img height="200" src="https://i.imgflip.com/65efzo.gif"  />
</div>

###

<div align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" height="30" alt="typescript logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/angularjs/angularjs-original.svg" height="30" alt="angularjs logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/materialui/materialui-original.svg" height="30" alt="materialui logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" height="30" alt="nodejs logo"  />
</div>

###
# Introduction

# Project Name : Angular-GeminiAI

# Prerequisites

Have  a web browser, code editor and git.
must be install node js in your system version Eg- "ts-node": "22.6.0"
like reference for node js https://nodejs.org/en


# Angular 15 

must be install angular cli in your system version like "@angular/cli" version "15.0.4"
and run command in Command line - npm install -g @angular/cli@15


# Getting Started
**Project Name - Angular-GeminiAI**
Guide users through getting your code up and running on their own system. In this section you can talk about-

## Clone the repository

git clone (rep link)
cd project name

## Install the NPM Package 
install the npm packages described in the package.json and verify that it works:-

npm install
npm start

## Development Server

Run ng serve for dev server. Navigate to http://localhost:4200/ The app will auto reload if you change any 
of the source code

## npm scripts

These are the most useful commands defined in package.json

npm start - run the Typescript compiler, asset copier and a server at the same time, all these in watch mode

npm build - runs the Typescript compiler and assets copier once.


# Angular Material UI Setup
This guide explains how to set up your Angular project to begin using Angular Material. It includes information on prerequisites, installing Angular Material, and optionally displaying a sample Material component in your application

Add Angular Material to your application by running the following command:
ng add @angular/material


# Create a custom Material Module
In this file material.module.ts we have manage for all material libraries




# Create Json Server 

npm install json-server

create a file db.json in Angular project folder
and Start up the JSON Server by typing this command into your terminal

json-server --watch db.json

This will run on "https://localhost:3000" by default.
you can change the port it's running on by specifying a different port number when starting the server using the --port flag

ng serve --port 4209

# Create Components

Here are the main project files that contain the application logic, I include component file that were generated by the Angular CLI ng new command :- 

--app
    |
    ---customer
    ---home
    ---login
    ---qa-generative
    ---register
    ---skelton (for loading ai response)
    ---pop-model
    ---user
    ---model

# Guard
The auth guard is an angular route guard that's used to prevent unauthenticated or unauthorized users from accessing restricted routes, it does this by implementing the CanActivate interface which allows the guard to decide if a route can be activated with the canActivate() method. If the method returns true the route is activated (allowed to proceed), otherwise if the method returns false the route is blocked.

The auth guard uses the authentication service to check if the user is logged in, if they are logged in it checks if their role is authorized to access the requested route. If they are logged in and authorized the canActivate() method returns true, otherwise it returns false and redirects the user to the login page.

using command 
 ng g guard guard/auth

# Service (AuthService)
create an service file for using this command line.

ng g s service/auth
Angular AuthService is well-structured for handling user authentication and interaction with a backend API.
--app
    |
    ---service
        |---auth.service.ts

# Service (GeminiService)
GeminiService is designed to interact with Google's Generative AI, specifically using a model named "gemini-pro". It maintains a message history using a BehaviorSubject, which allows you to track and emit messages from both the user and the bot. 

Create an Service file for gemini 
ng g s service/gemini

--app
    |
    ---service
        |---gemini.service.ts

install for gemini in your project for using command line
npm i @google/generative-ai

import { GoogleGenerativeAI } from '@google/generative-ai'; inside qa-generative component.

constructor() { this.generativeAI = API KEY }






















