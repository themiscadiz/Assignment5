<!-- Every README should start with an H1 -->
# Assignment5 - Using NEDB 
<!-- A one sentence description of the project or assignment -->
This assignment is a continuation of assignment 4. A voting system for animals. Instead of using a saved JSON file, I implemented a database with NEDB, following Joey's simple express API [tutorial](https://github.com/joeyklee/simple-express-api).

Still only one option, the cat.

**I intend to add more animals for the final version, and submit that as my final project for this course.**


![img1](https://github.com/themiscadiz/Assignment5/blob/master/images/12.png?raw=true)

<!-- It is good practice to add an about or summary -->

<!-- It is essential to describe how to set up your project -->
## Setup
To setup the project you need access to a computer and the internet. 
To be able to see the website you can go to [Glitch Website](https://glitch.com/~themiscadiz-assignment5)

<!-- Any knowledge or tools you will need before hand -->
## Prerequisites

The following prerequisites are necessary:

A text editor - like VS Code
Terminal or Command line.

<!-- any installation needs should be defined -->
## Installation
You need the express, path, fs, nedb, and nodemon libraries from npm

<!-- Notes about the deployment -->
## Deployment

To locally host your website (in case of Mac):

1. Download the Code to your computer.
2. Open the Terminal
3. Type cd (don’t forget the space)
4. In Finder, navigate to the folder and Drag and drop into the Terminal.
5. Type <pre><code>npm start</code>
6. Server should launch, and you should see the correct ip address to navigate to. Something like this: **localhost:3000**  

## Built with
* [Nodejs](https://nodejs.org/en/)
* [VS Code](https://code.visualstudio.com/)
* [Github](https://github.com)
* [Glitch](https://glitch.com/)
* [Postman](https://www.postman.com/downloads/)

***
***
***

<!-- For your assignments you might consider  -->
# Notes & Process
My goal in thi assignment was to use NEDB, Postman, and how to use PUT correctly.

I started by following Joey's Simple Express API tutorial to understand the process of switching over from JSON to the NEDB database. The tutorial was good to follow and I was able to use CRUD correctly. Also, I was very interested in using p5.js for the frontend, since I am familiar with it.

After doing this tutorial, I decided to use NEDB instead of MongoDB, it seemed easier for me right now. Hopefully later I'll be able to use MongoDB.

![img](https://github.com/themiscadiz/Assignment5/blob/master/images/1.png?raw=true)

I was able to implement the NEDB database into my own code from last week's assignment. Although, I had a lot of difficulty interfacing with the frontend, I think because an async issue. I tried to access the DB and send the votes to the html but my getVotes function returned **unidentified**. I finally got it to work, but I'm still not exactly sure how. **I'm planning to return to this code to figure it out.**

I also left a ton of commented out code. I haven't deleted it because there might be something useful there still. Will clean later.

### NEDB and Postman
It was actually pretty simple to implement. Following the tutorial was very useful. Using Postman helped me quickly test my code, instead of using the terminal of writing more code just for testing.
![img](https://github.com/themiscadiz/Assignment5/blob/master/images/3.png?raw=true)

![img](https://github.com/themiscadiz/Assignment5/blob/master/images/8.png?raw=true) 


### Implementing PUT
For last week's assignment, I had trouble implementing PUT, but using the tutorial and Postman I was able to update my database with no problem.
![img](https://github.com/themiscadiz/Assignment5/blob/master/images/9.png?raw=true)

### Getting data from the DB, Async and promise
I had a lot of trouble getting the data into local variables in my app.js file. I think it has something to do with the async functions, await and promises. When I called the function to get the data it first returned as unidentified, then I thought to turn my getVotes() function into an async and use await, but I got errors. 

I'm not sure but I think I'm calling the database directly from the html? This part is still very confusing for me but I will continue to work on it for my final project.

![img](https://github.com/themiscadiz/Assignment5/blob/master/images/2.gif?raw=true)

To see a detail video:
[click here](https://github.com/themiscadiz/Assignment5/blob/master/images/Weird-db-frontend-working.mov?raw=true)


### Deploying to Glitch
I was finaly to deploy to Glitch by using the correct url (https://themiscadiz-assignment5.glitch.me/) instead of localhost://

![img](https://github.com/themiscadiz/Assignment5/blob/master/images/1.gif?raw=true)

![img](https://github.com/themiscadiz/Assignment5/blob/master/images/13.png?raw=true)



## Challenges, Struggles & Questions
1. Getting data from the DB and storing it in a variable.
2. Async function maybe?

<!-- References for resources and inspiration -->
## References
**Class Material**

[simple-express-api - A simple frontend and static web server](https://github.com/joeyklee/simple-express-api) by [Joey Lee](https://github.com/joeyklee)


[Introducing Postman](https://github.com/joeyklee/simple-express-api#introducing-postman) by [Joey Lee(https://github.com/joeyklee)

**Online References**
[MDN await](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/await)

Cat picture from [Unspash](https://unsplash.com/s/photos/cat)


## Authors
* [Themis Garcia](https://github.com/themiscadiz) -- NYU ITP student
