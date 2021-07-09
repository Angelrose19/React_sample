# React ES6

ES6 stands for ECMAScript 6.

ECMAScript was created to standardize JavaScript, and ES6 is the 6th version of ECMAScript, it was published in 2015, and is also known as ECMAScript 2015.

React uses ES6, and you should be familiar with some of the new features like:

 * Classes
 * Arrow Functions
 * Variables (let, const, var)

 ## Classes

ES6 introduced classes.

A class is a type of function, but instead of using the keyword function to initiate it, we use the keyword class, and the properties are assigned inside a constructor() method.

Example
A simple class constructor:
```javascript
class Car {
  constructor(name) {
    this.brand = name;
  }
}
```
Example
Create an object called "mycar" based on the Car class:
```javascript
class Car {
  constructor(name) {
    this.brand = name;
  }
}

mycar = new Car("Ford");
```
**Note** : The constructor function is called automatically when the object is initialized.

### Method in Classes
You can add your own methods in a class:

Example
Create a method named "present":
```javascript
class Car {
  constructor(name) {
    this.brand = name;
  }
  
  present() {
    return 'I have a ' + this.brand;
  }
}

mycar = new Car("Ford");
mycar.present();
```
### Class Inheritance
To create a class inheritance, use the extends keyword.

A class created with a class inheritance inherits all the methods from another class:

Example
Create a class named "Model" which will inherit the methods from the "Car" class:
```javascript
class Car {
  constructor(name) {
    this.brand = name;
  }

  present() {
    return 'I have a ' + this.brand;
  }
}

class Model extends Car {
  constructor(name, mod) {
    super(name);
    this.model = mod;
  }  
  show() {
      return this.present() + ', it is a ' + this.model
  }
}
mycar = new Model("Ford", "Mustang");
mycar.show();
```
The **super()** method refers to the parent class.

By calling the **super()** method in the constructor method, we call the parent's constructor method and gets access to the parent's properties and methods.

## Arrow Functions
Arrow functions were introduced in ES6.

Arrow functions allow us to write shorter function syntax:

Before :
```javascript
hello = function() {
  return "Hello World!";
}
```
With Arrow Function:
```javascript
hello = () => {
  return "Hello World!";
}
```
It gets shorter! If the function has only one statement, and the statement returns a value, you can remove the brackets and the return keyword:

Arrow Functions Return Value by Default:
```javascript
hello = () => "Hello World!";
```
Note: This works only if the function has only one statement.

