# react-to-do-app

React Redux application for managing our daily to-do-list.


A complete Single-Page-Application (SPA) created using React JavaScript library. We have used Redux for state management and Bootstrap for styling the UI. We are interacting with a RESTful API which is protected using JWT.


Another thing to note is, we have not used any 3rd party library such as thunk/saga for performing async operations. Instead we have created own custom API redux middleware. For any medium to large application, leveraging redux middleware helps in centralizing common tasks (or cross cutting concerns) such as API calls, exception handling and logging.

And  We have used MongoDB as the database and mongoose as the ORM library which makes it easier to interact with MongoDB.
Apart from this, we have used JSON Web Token (JWT) to add authentication. Using JWT, we can protect certain endpoints and ensure that user must be logged-in to access those.

## Setup and Installation

1. **Clone the React app repo from GitHub**
   ```sh
   git clone https://github.com/ravira03/to-do.git
   ```

2. **Install npm dependencies**
   ```sh
   cd to-do
   npm install
   ```


3. **Setup MongoDB**

   There are lots of options available to have a running MongoDB instance:
   - a typical way is to download the community edition from [here](https://www.mongodb.com/download-center/community) and install locally on the machine
   - another option is to spin-up an instance on the cloud. Here are step-by-step instruction for that - [Get Started with Atlas](https://docs.atlas.mongodb.com/getting-started)
   - another option is by running a mongodb docker container. If docker is installed, its simply a matter of running single command to spin-up a database instance:
     ```sh
     docker container run --name mongodb -d -p 27017:27017 mongo
     ```



4. **Run npm start to start the application**
   ```sh
   npm start
   ```
   this runs the application at port 3000 and we can access from http://localhost:3000

   And open another terminal and change the directory to 
   ``` 
    cd to-do-api 
   ```
   And run npm start. this runs at port 3300 and hence all enpoints can be accessed starting from http://localhost:3300




