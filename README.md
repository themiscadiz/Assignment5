<!-- Every README should start with an H1 -->
# Assignment5 - Using NEDB 
<!-- A one sentence description of the project or assignment -->
This assignment is a continuation of assignment 4. A voting system for animals.Instead of using a saved JSON file, I implemented a database with NEDB. Following Joey's simple express API [tutorial](https://github.com/joeyklee/simple-express-api).

Still only one option, the cat.

I intend to add more animals for the final version, and submit that as my final project for this course.


![img1]()

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

I started by following Joey's Simple Express API tutorial to understand the process of switching over from JSON to the NEDB database. The tutorial was good to follow and I was able to use CRUD correctly. 

I was very interested in using p5.js for the frontend, since I am familiar with it.

After doing this tutorial, I decided to use NEDB instead of MongoDB, it seemed easier for me right now. Hopefully later I'll be able to use MongoDB.

![img]()

I was able to implement the NEDB database into my own code from last week's assignment. Although, I had a lot of difficulty interfacing with the frontend. I think becuase if the async issue. I tried to access the DB and send the votes to the html but my getVotes function returned **unidentified**. I finally got it to work, but I'm still not exactly sure how. But I'm planning to return to this code to figure it out.

I also left a ton of commented out code. I haven't deleted it because there might be something useful there still. Will clean later.

### Understanding NEDB
Following the Foundations Guide from the class, I was able to  understand how to interact with node through the terminal.

![img]()

In my first attempt, I started to use the Horoscope.js. But while I was diving into the material, I noticed that I actually wasn't going to explore the fundamentals concepts of this assignment. 

![img]()

However, when I tried to start the assignment I realized I needed help understanding how to interact with node.js, it is not the typical way I have used js... after that, I understood it more as an invisible, backend that I was only able to see it running in the terminal. Not as a console log on the browser.

### Designing the website
After I finally got the concept of the assignment. I started to design my website and decided to start with the frontend. I sketched the design. After simplifying, I eliminated the other animals, to focus on the basic functionailty.

![img]()

### Creating an API
Creating the API was the most time consumming part of the assignment. Even having the class material, it was hard for me to understand how to apply it into my own project. The challenges starting for even understanding were node runs and what libraries I needed to get the data.
![img]()

Another challenge was to access the frontend files. I tried to use <code> const indexLocation = path.join(__dirname + "/frontend/")</code> but didn't work as espected. I had to put the css and js code inside the html file to be readable.

From the beggining I was confused how to get the path to read the api numbers that I was putting from the server. For this I follow a Express website example using .Router()

![img]()

However, after many attempts a was able to listen and see through the terminal the increasing value from the api/cat.

![img]()


### Accesing the API

After I was able to see the information updating in the server from the app.js, I started to try to acces this information from the API (as last week assignment). Although I had difficulties I felt more confortable with the similarities from last week's assignment. 

![img]()

I was able to see the information updating in the website even when I refresh the site. However, when I close the server, the counter of votes started from 0, because I was not storing the information anywhere. Is because of this the importance of having a json database, to be able to store the information even if the server closes. 

### JSON database

I created the json file (votes.json) to put the votes information and I prepopulated with a json object. In app.js I created a function with fs.library to acces the json file. In that way, I was able to read the json file and write to it using those functions.

In the function getVotes() I read the json file and return the votes value.

In function updateVotes() I updated the cat variable, I created a new json object with the updated cat variable. And then I overwrite the object in the json file.

To updated the cat variable with the last value of votes from the json file.
<code> let cat = getVotes();</code>

**In this gif I recorded when the json file is been updated by the backend when I clicked the image. Even if I refresh the website and the server, the counter of votes is going to show the quantity of votes accumulated.** It's simple but I'm SUPER PROUD of this.

![img]()

To see in better resolution, here's is a [link to a video]() 


### Deploying to Glitch
I wasn't really able to deploy the assigment through Glitch. I tried change the http to https (and vice versa) and make sure that I was using <code> start: node app.js</code> in the package.json, but it still didn't work. However, when I still have the server on locally on my computer, I see changes in the json file when I pressed through the Glitch site. I was able to find and open the terminal in Glitch, but wasnt able to understand the errors that I recieved.

![img]()

![img]()




## Challenges, Struggles & Questions
1. Understanding the nature of backend, node, and how to work with it.
2. How to request the information of different votes from different animals? Do I have to use an async function in the <script> for each animal?
3. Deployment of website in Glitch
 

<!-- References for resources and inspiration -->
## References

[simple-express-api - A simple frontend and static web server](https://github.com/joeyklee/simple-express-api) by [Joey Lee] (https://github.com/joeyklee)
[Introducing Postman](https://github.com/joeyklee/simple-express-api#introducing-postman) by [Joey Lee] (https://github.com/joeyklee)

[MDN await](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/await)

Cat picture from [Unspash](https://unsplash.com/s/photos/cat)

Class Material

## Authors
* [Themis Garcia](https://github.com/themiscadiz) -- NYU ITP student
