# :wave: The Basics of P5 

## 🤓 Course overview and learning outcomes 💻 

In this assignment we will be exploring Objects. To do this we will be simulating dice 🎲🎲🎲🎲🎲🎲 and how they roll. 
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


  
## 📚  Resources / References
* [Mozilla Working with objects Documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects)
