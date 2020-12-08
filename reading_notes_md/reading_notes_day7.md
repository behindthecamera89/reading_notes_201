# **Object-Oriented Programming, HTML Tables**
## Read [Domain Modeling](https://github.com/codefellows/domain_modeling#domain-modeling)

- object-oriented model stores data properties and encapsulates behaivors in methods
- A domain problem that is articulated well can verify and validate the understanding of specific problems
- Object Orienting at a basic level
  - The new keyword instantiates an object
  - the constructor function initializes properties inside that object using this variable
  - the object is stored in a variable for later use
- Practiced some code in the console - wrote this out
  - 'use strict';

var EpicFailVideo = function(epicRating, hasAnimals){
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}
EpicFailVideo.prototype.generateRandom = function(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}
var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail.generateRandom(1, 5));
console.log(corgiFail.generateRandom(1, 5));
- generateRandom is a "Method"
- min and max are parameters 
- "When parkourFail is asked to run the generateRandom() method, it searches through all of its own methods. When it doesn't find the generateRandom() method there, parkourFail then searches through all of the methods on its prototype object. When it finds the generateRandom() method on its prototype object, parkourFail calls the method, passing in 1 and 5 as the arguments. The generateRandom(1, 5) method runs and returns a random number between 1 and 5. The exact same process happens for corgiFail too."
- domain modeling is the process of creating a conceptual model for a specific problem



## From the Duckett HTML book:
## Chapter 6: “Tables” (pp.126-145)
- Tables represent information in a grid format
- basic tables structure 
  - <table>
      <tr>
        <td>15</td>  
- Above is used to add a table
- table headings <th scope="row">
- <td colspan="3"> extends the width of a column 
- <td rowspan'2> expandes the row
- below is used for long tables
- headings of a table should sit insie the <thead> element
- <tbody> the body sits inside here
- <tfoot> the fotter belongs inside here


## From the Duckett JS Book:
## Chapter 3: “Functions, Methods, and Objects” (pp.106-144)

- Creating an object  - constructor notation 
- use dot notation to update the value of properties
- object constructors can use a function as a template
- create multiple objects on the same page
- craete objects, then ad properties to it and methods
- this. is a keyword it refrences the function you are in
- store data
- arrays are objects
- functions allow you to group a set of related statements together that represent a single task
- functions can take parameters (information needed to do a job) and return a value
- an object is a series of variables and functions that represent something from the world around you
- in an object, variables are known as properties that represent both the browser window and the document loaded into the browser window
- javascript has built in object such as strings, number, math, date. these offer functionality that help you write scripts
- arrays an dobjects can be used to create complex data sets


[home](/README.md)