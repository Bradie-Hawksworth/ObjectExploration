# :wave: The Basics of P5 

## 🤓 Course overview and learning outcomes 💻

In this assignment we will be exploring Objects. To do this we will be simulating dice and how they roll. 
.
.
.
Sorry I couldn't resist. We're actually going to be moving on from dice (🙌). The following is a description of objects taken from the Mozilla documentation (a link for this can be found at the bottom of this document).
*'JavaScript is designed on a simple object-based paradigm. An object is a collection of properties, and a property is an association between a name (or key) and a value.'*

Objects build on from the work we were doing with variables. Similar to arrays, objects can hold many different items of information this includes variables, arrays and even functions. Variables within an object are known as the objects attributes, functions within an object are known as methods.

The following syntax is an example of an object being created.
  
  ```js 
    let exampleObject = {
          exampleAttribute : 'value',
          exampleAttribute2 : 2,
          exampleMethod : function printExampleAttribute() {
            print('An example of a function being declared within an object');
          }
    }
   ```

Note the similarities between the syntax of an object and an array. The main difference is that within an object we have to provide a name (key) for the data within the object. 

Objects are regularly used to model 'things' from customers to cars, objects and classes (we'll move on to classes in a future assignment) are the mechanisms we use to encapsulate all information relative to the given thing.

## Task - Think about a 'thing' What attributes does the 'thing' have? What can the 'thing' do?

Think about either an object or a pet or a person. What attributes could you give that object in your program? 

Create the object within your program or add some notes to your project describing the intent of your object.

## Accessing attributes and methods of an object

In order to access the methods and attributes of an object, the dot notation should be used. The dot notation takes the following format.

```js
let exampleObject = {
          exampleAttribute : 'value',
          exampleAttribute2 : 2,
          exampleMethod : function printExampleAttribute() {
            print('An example of a function being declared within an object');
          }
    }
    
//This is an example of how you are able to access the attributes within an object
exampleObject.exampleAttribute;

exampleObject.exampleAttribute = 'new value';

//The following is an example of an objects method being called.
exampleObject.exampleMethod();
```

## Task - Implement the 'thing'!
Thinking back to the 'thing' you thought about in the previous task. Can you call it's functions to make it do something? If you haven't already, try and implement the object in code and try and call it's methods.



<details>
  <summary> Adding the if statement </summary>
  My process can pe found below. If you don't want to see my process, continue on. You can always come back and see how my process compares to yours. 
  <details>
    <summary> My intent </summary>
    
     * I will create a global variable to remember the value that needs to be drawn on screen
    
     * I will need to add an If statement to the Draw() Function in order to draw the correct dice face
    
     * I will need some mechanism to generate a random number that the dice face on the screen will reflect
    
  </details>
  
  For my implementation I am going to use a Global variable to remember the value that has been rolled. This is what I will use within my If statement to evaluate my true clauses. This may seem strange but because of the Draw() function being called constantly, the drawing is constantly refreshed in the background. If I was to call the function just once, I wouldn't see the dice after the first refresh.

  The following screenshot show the global variable implementation
![image](https://user-images.githubusercontent.com/67816866/150936407-5a8da22d-443a-4ad3-8cd8-2955d42e8a51.png)

  This variable has been created outside of any function and using the var keyword.

  Now that I have a location to store my dice roll, I can start to think about the if statement. 

  In the example I have 6 dice functions defined. These represent each face on a 6 sided dice.

  * Why has this variable been created where it has?

  * Why haven't I used the const keyword to describe this variable? 


  ## My first attempt at an If statement to draw the dice face.
  The following screenshot show the first implementation of my If statement. This implementation is designed to draw the face of the dice representing 'one' when dice value is equal to one. 
  ![image](https://user-images.githubusercontent.com/67816866/150938825-03bc521e-8b0d-49c4-ab1a-ca8cc7058f6a.png)

  🧐 'Hmm... This doesn't seem to be outputting anything on the screen...' Why does the example in the above screenshot not seem to be outputting anyting? Write down some suggestions to make the dice output to the screen.
  
  
  ## Task - Make the dice appear on the screen
  Add screenshots of the changes you have made to make the dice appear on the screen.
  
  
  
  ## Task - Expand the If statement
  Add more conditions to the If statment. Are you catering for all possible dice face?
  Add a screenshot of your changes. 
  
  
  How did you test these changes?
  
  
  ## Extension Task - Can you add a button to change the value of the dice? 
  [p5.js Button Documentation](https://p5js.org/reference/#/p5/createButton) Using this documentation, can you add a button to change the value of the dice being displayed? 

  Take a minute and think about this, what needs to change? 

  *Write down the process you want the user to do in order to 'roll the dice'.* What does this include? 
  
  
</details>
  
## 📚  Resources / References
* [Mozilla Working with objects Documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects)
