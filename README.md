# :wave: The Basics of P5 

## 🤓 Course overview and learning outcomes 💻

In this assignment we will be exploring Objects. To do this we will be simulating dice and how they roll. 
.
.
.
Sorry I couldn't resist. We're actually going to be moving on from dice (🙌). The following is a description of objects taken from the Mozilla documentation (a link for this can be found at the bottom of this document).
*'JavaScript is designed on a simple object-based paradigm. An object is a collection of properties, and a property is an association between a name (or key) and a value.'*

Objects build on from the work we were doing with variables. Similar to arrays, objects can hold many different items of information this includes variables, arrays and even functions. Variables within an object are known as the objects attributes, functions within an object are known as methods.

Pay close attention to the functions we are calling. All of the function signatures follow the same pattern. 
  
  ```js 
    let exampleObject = {
          exampleAttribute : 'value',
          exampleAttribute2 : 2,
          exampleMethod : function printExampleAttribute() {
            print('An example of a function being declared within an object');
          }
    }
   ```
This may be different to the implementation within your project and doesn't really matter if you are using the example you have created.

When we roll a dice a random outcome is provided by the result on the face of the dice. This assignment will focus adding this functionality to our dice. Before continuing on, take a few minutes to plan out how this will be done in your code. 

* Think about the tools you have learnt over the past couple of assignments. What do you need to know or remember in order to produce a random dice face? 


## If Statements
[Mozilla If...Else Documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/if...else) This link will take you to the Mozilla documentation regarding if...else statements. 

If statements are executed if the condition returns a true value. This is known as a truthy value. (Documentation on truthy and falsy values can be found here [Mozilla truthy and falsy Documentation](https://developer.mozilla.org/en-US/docs/Glossary/Truthy).

The syntax for an if...else statement is shown below.

```js
  if (condition) {
     statement1
  } else {
     statement2
  }
```
The relational operators documentation can be found [here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators#relational_operators). These are some of the most common operators used in conjunction with the If statements.



## Task - Add an If...Else statement to the Draw() Function in your sketch.
Before we add an If...Else statement to the Draw() function we need to think about what we want to check is resulting as true.

* What do we want to check is true?

Think in terms of the dice, we have several different faces. How are we going to determine what face we want to display on the screen? 


*Think about the previous section where you wrote down what you may need to simulate rolling a dice.*



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
