# Adslots_manager
Administrator for managing Ad Slots

Libraries used:
React, Webpack, SASS

Platform:
NODE, NPM

Running App (Demo): http://18.209.16.90:8081/ (It will be slow the first time)

Steps to install and run locally:

    git clone https://github.com/vikaskulkarni/Adslots_manager.git
    cd Adslots_manager

    npm install

Production Mode

    npm run build
  
The above step will create a dist folder. index.html can be run in any web server.
Install http-server globally

    npm i -g http-server
    cd dist
    http-server
  
Navigate to http://localhost:8081/. In this mode, the code changes are NOT automatically loaded. Make sure the underlying service layer is running on 8080 that serves the APIs
  
Development Mode

    npm run start-dev
  
Navigate to http://localhost:65132/. In this mode, the code changes are automatically loaded. Make sure the underlying service layer is running on 8080 that serves the APIs


Looking at the project structure:
components

    This contains the reusable components like header, footer, table, search, select, form, toggle. These are standalone components that can be used by any pages by passing required props.

containers

    This contains the Application container, App.jsx that embeds all the required components to design the page. The application has;
    - header
    - table to list the Ad slots
    - form to show the Ad details and create, edit

service

    This is common api layer that uses 'axios' library to make server calls
