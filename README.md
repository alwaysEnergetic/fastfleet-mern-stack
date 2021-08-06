<h1 align="center">
  <img alt="Fastfeet" title="Fastfeet" src="./backend/img/logo.png" width="300px" />
</h1>       
          
<p align="center">       
  <a href="#rocket-sobre-o-desafio">about the challenge</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp; 
  <a href="#Backend">Backend</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;  
  <a href="#Frontend">Frontend</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;   
  <a href="#Mobile">Mobile</a> 
</p>         
           
      
## :rocket: about the challenge 

The application consists of a fictitious carrier system called FastFeet. It is a complete application involving back-end, front-end and mobile, and that is part of the certification challenge of the bootcamp Gostock da **[rocketseat](https://rocketseat.com.br/gostack)**.

<img src="/prev/Prev01.png">
</br>
  
<img src="/prev/Prev02.png">
</br> 
  
<img src="/prev/Prev03.png"> 
</br>
    
 
## Tools  

:whale: Docker 

    In the project, the docker tool was used to create the database.
     Access the documentation (https://docs.docker.com/get-docker/), to install the version according to your
     operational system.

   
  Create and upload a database (Postgres):
 
     $ docker run --name fastfeet -e POSTGRES_PASSWORD=fastfeet -p 5432:5432 -d postgres
     $ docker start fastfeet

  Create and upload a Redis database:
 
     $ docker run --name redisfastfeet -p 6379:6379 -d -t redis:alpine
     $ docker start redisfastfeet


  Installing PostBird, an application to view database information.

    You can access the documentation:(https://www.electronjs.org/apps/postbird) for the installation according to your operating system.

  Accessing postbird, fill in the access data, host, port, username and password according to the database created via docker.
 
      After that, inside postbird, create a database named fastfeet.
      
      
 ## 💹 Backend 

    $ git clone https://github.com/the-one-who-knoccks/FastFeet-Master.git

  Accessing the directory:

    $ cd FastFeet-Master/backend

  Installing dependencies.

      run the yarn or yarn-install command to install the dependencies.


   Migrations e seed.

    Run yarn sequelize db:migrate to create migrations and yarn sequelize db:seed:all to create seeds.
    
   .env

     Change the .env.example file to .env and inform the parameters according to your development environment.

 Starting the server.

    To start the server, run the yarn dev command.
    
  Email server.

    To run the email server, run the yarn queue command.
    

## ⚛️  Frontend

  Installing dependencies.

      Run the yarn command or yarn install.
 
 Starting the web application server.
 
      To start the application server, run the yarn start command.


## ⚛️ Mobile

  Setting localhost and ip in Reactotron

    Access the mobile folder and navigate to the src/services folder and in the api.js file, set the url/localhost of your emulator. Then go to src/config/ReactotoronConfig and change the part ".configure({ host: 'ip of your machine here })" After that, run the command below to install the dependencies: 
    
    yarn ou yarn install.


   Once you have your emulator or cell phone connected, open the terminal in the Mobile_Gobarber folder and run the command:
    
    $ react-native run-android ou run-ios.

   Then after finishing the installation, run: 

    $ react-native start ou yarn start no terminal.
    
# Observation 

    Application tested on Android only.
    
