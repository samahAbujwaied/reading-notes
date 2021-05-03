# Domain Modeling
![](https://miro.medium.com/max/5000/1*UuZRQ57iPmEKsY5wsgGBLA.jpeg)
**Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.**
**A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.**

## Define a constructor and initialize properties

![](https://i.imgur.com/IduZcBy.png)

**To define the same properties between many objects, you'll want to use a constructor function. Below is a table that summarizes a JavaScript representation of an EpicFailVideo object.**

|Property  |   Data    | 	Type  |
|----------|-----------|----------|
|epicRating| 	1 to 10| 	Number|
|hasAnimals|true or false| 	Boolean|



### Here's an implementation of the EpicFailVideo constructor function.
```var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}
var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);
console.log(parkourFail);
console.log(corgiFail);

```
> As you can see, the constructor function is defined using a function expression. In other words, the variable EpicFailVideo is declared and then assigned a function with two parameters called epicRating and hasAnimals.

> When the function is called, the data inside these parameters are stored inside the this.epicRating and this.hasAnimals properties respectively. Storing data within properties ensures any newly created object can access that data later.

> After the constructor function definition, two objects are instantiated with the new keyword and their properties are initialized by calling the EpicFailVideo constructor function. After being instantiated and initialized, these objects are stored inside the parkourFail and corgiFail variables.

> Finally, the two newly created objects are logged to the console.

![](https://camo.githubusercontent.com/55928963ae0dc919186799ab35c1cd669724ddbeb0658d0ca4b9e79b38e1804e/68747470733a2f2f692e696d6775722e636f6d2f47326250456c462e706e67)

## Generate random numbers
![](https://i.stack.imgur.com/nIHGJ.png)

# Tables
* How to create tables
* What information suits tables
* How to represent complex data in tables

### basic Table structure
* table tag 
* tr tag 
* td tag 
* Table headings 
    * th tag 

![](https://www.thedataschool.com.au/wp-content/uploads/2018/10/HTML-table-.png)

* spanning columns
* spanninag rows

![](https://i.stack.imgur.com/Uvzmu.jpg)

### long Tables
* thead tag 
* tbody tag 
* tfoot tag

### WidTh & spacing for table
![](https://i.stack.imgur.com/He8mJ.png)

### border & background for table
![](https://lh3.googleusercontent.com/proxy/6bMuve8YOce1IFqx0pbmtPwVIovnS0BwlFHce2TcBvxHaUW07_drsCUlciejSZpRxw3sTOhEZma4Xiu7v_Po6Th4VHS6y8GZSwZM6ie3) 

## Updating an object in JS
**To update the value ofproperties , use dot notation or square brackets they work on objects created on objects created using literal or constructor notation . To delete a property use the delete keywword.**

![](https://i.stack.imgur.com/N1odX.png)

## Updating an OBJECT
![](https://www.codegrepper.com/codeimages/how-to-change-object-value-in-javascript.png)

## Creating many OBJECT : constructor notation
![](https://miro.medium.com/max/4096/1*KYFTHD69xtacnwbKRyFuqQ.png)

## Creating Objects Using Constructor syntax
![](https://csawesome.runestone.academy/runestone/books/published/csawesome/_images/worldConstructors.png)

## Crating & access OBJECTS constructor notation
![](https://miro.medium.com/max/1720/1*NnC4CgrM9CLzYflkmEZLQw.png)

## Adding and removing properties
![](https://flaviocopes.com/how-to-remove-object-property-javascript/delete-object-property.png)

## This (IT IS A KEYWORD )
![](https://www.tutorialsteacher.com/Content/images/oo-js/this-global.png)

# Best Regards 