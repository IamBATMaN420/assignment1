---
title: "Mastering JavaScript OOP: A Comprehensive Guide to Object-Oriented Programming"
seoTitle: "Mastering JavaScript OOP: A Comprehensive Guide to Object-Oriented Pro"
seoDescription: "Learn the fundamentals of JavaScript Object-Oriented Programming (OOP). Explore key concepts like classes, inheritance, encapsulation, and polymorphism ."
datePublished: Sat Nov 30 2024 07:21:22 GMT+0000 (Coordinated Universal Time)
cuid: cm43ug7e8000209lh7szvexy0
slug: mastering-javascript-oop-a-comprehensive-guide-to-object-oriented-programming
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1732951182425/4d150c27-fb42-4fd3-a985-89c39c02d89f.webp
tags: js, javascript, backend, typescript, functional-programming, frontend-development, oops

---

**Description:**  
Learn the fundamentals of JavaScript Object-Oriented Programming (OOP). Explore key concepts like classes, inheritance, encapsulation, and polymorphism with practical examples to enhance your coding skills.

---

so let’s start:→

THE MILLION DOLLAR question is :-&gt;

### **Is Javascript a "OOP" based language or a "prototype" based language ?**

so the answer is bit complicated js at first meant to be made for "prototype" based later they tried to make js as "oop" based. But they realised then they have to change the whole lang and make "many changes". **So. they decided to make "OOP" based but under the hood they still use "Prototype".**

so we must have the basic knowledge of “Protoype”.so in the first place we have to know about “OOP”.

---

**real life idea of” prototype” and “object“ :→**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1733415993581/bf400fd8-3499-4cdb-8eea-adb77707cab4.png align="center")

---

## 1\. All about “Prototype“:→

So to start with it, OOP , we have to start with “prototype”. Now, we have to go through basic console output in the browser.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1733325701488/e8dbca45-7389-4da3-8466-f6d73d58e393.png align="center")

Now, we will click on arrow button.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1733325777750/69712356-c74e-4508-8edf-a19411896525.png align="center")

that’s the example of the “prototype“. Here is the properties of the object. We must have to note that “prototype“ part.

---

## a&gt; by dendor (\_\_proto\_\_) :→

so let’s see with an example :→

```javascript
// let us make a object
// 3 object has different properties let's make some protype with "dendon[object.__proto__]"
let ayush={
  eyes:2,
}
let piyush={
   ears:2,
}
let manus={}
//
console.log(`ayush`,ayush.__proto__);
```

let’s see the output of it :→

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1733328808124/3e365adc-438c-48ec-86e9-259a6725d41f.png align="center")

see the output but is we gave the same the code browser the result will be different . cz those are the basic or the actual or “deafault“ property of the “object“. let’s explore that too.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1733329492739/7a7d432b-36f9-454a-bf92-4f6eb844034c.png align="center")

so why it’s happening the answer is it’s the by default property of “object“ or “prototype” injected by browser. that was defined previously.

---

so let’s see another thing about ”Prototype” where the property will be injection by us try to understand the structure.

```javascript
// let us make a object
// 3 object has different properties let's make some protype with "dendon[object.__proto__]"
let ayush={
  eyes:2,
}
let piyush={
   ears:2,
   __proto__:ayush,
}
let manus={}
//
console.log(`piyush`,piyush.__proto__);
console.log(`piyush ears`,piyush.ears);
```

now here what we are doing is making the protype with some modification . in this section the code is same here we will try to make the “prototype“ of “ayush” and inject it to ”piyush” and try to access thatand see the output . so let’s see the output :→

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1733330288919/817d99c8-9932-46c5-9602-fb2acb4b6d0b.png align="center")

now after seeing this we will try to understand the “prototype“ and accessing that by a diagram.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1733330874060/4d45e4e6-8a5e-4a68-ba62-d32babc653b1.png align="center")

that’s how prototypes arebeing made but there are more ays to make it without dendon. let’s see them

1&gt; by dendon\[object.\_\_proto\_\_\] (prv form)

2&gt;setprototypeof() and getprotypeof() methods.

---

## **b&gt;setPrototypeOf() and getPrototype0f() :→**

t**he syntax of setPrototypeOf() is** setPrototypeOf()**(new obj,old obj) and in** getPrototype0f\*\*(which object’s property we want to find),\*\*

here us an example with code part where we try to understand it more better :→

```javascript
let ayush={
  eyes:2,
}
let piyush={
   ears:2,
}
Object.setPrototypeOf(piyush,ayush);
console.log(Object.getPrototypeOf(piyush));
```

## note:→ there is a mistake i do alot that’s writing it “object” instead *“Object”.* so we have to use “*Object”.*

here is the output :→

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1733415799665/ac3bb627-a28c-48aa-9f94-13adf977e73f.png align="center")

more over here completed the “master-class on prototypes” and move to “OOP“ concepts.

---

# 2&gt;Functional constructor :→

here we make the “**functional constructor“ to make “objects” in js.**

so let’s learn around “Functional constructor” :→

in this example we will learn about “making: functional constructor”

prerequisite :→ js foundation (“this” keyword context wrt obj)

```javascript
function Car(name,version) {
  this.name=name;
  this.version=version;
  this.description=function(){
    return(`this is my ${this.name}`)
  }
}
 const car1= new Car("thar","4");
 console.log(car1);
 console.log(car1.description());
```

there is many this we can talk and lets go through with that

1&gt;In “Functional constructor“ we first have to write “***function***” and name it as we want but must start with ***<mark>capital alphabet</mark>*** , just like in the example i have made ***“Car” function.***

2&gt;so in the function we have function parameter. and that must be stored in a “***variable***”. It’s okay. right? what’s new ?yes there is some things to note :→ here parameter are stored are by ***<mark>“this“</mark>*** keyword, to see it we have to see the example.

3&gt; there is ***<mark>“new”</mark>*** keyword that show that the new object is being made. an then we storing it another variable then console.log() that.

4&gt; even for making the function in the “function constructor we have to use ***<mark>“this” </mark>*** keyword for the context.

---

### prototype with functional constructor :→

let’s see this with examples :→

```javascript
function Fruit(name,taste){
  this.name=name;
  this.taste=taste;
}
Fruit.prototype.price="high"
const mango = new Fruit("mango","sweet")
console.log(`the price of mango is ${mango.price}`);
console.log(mango);
```

here we make the prototype is made by \[.prototype\]

so we have to know “what is prototype?”… so why can’t we use the previous ones. The answer is they are only valid for “objects“ and here we define it for “function“.

So, fruit.prototype =&gt; here we inherit the prv property of the “fruit” and then make a new property by “.price” and add that in the function.

---

# 3&gt; Object and inheritance :→

from here we will enter to the space of ***“object-oriented programing”…***

here is a pictorial representaion :→

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1733583270933/ced16fad-dd3f-4478-8873-02fab212a921.png align="center")

here we will the object-orientend part we will see the protypal chain an how can we make “inhertance” and “class” in javascript . Under the hood they still use “prototype”.

```javascript
let car = {
  model: "lamborgini",
  car: "a4",
  start: function () {
    return `${this.model} is made by ${this.car}`;
  },
};
console.log(car.start());
//functional constructor
function Bike(amount,ride) {
  this.amount = amount;
  this.ride = ride;
}
Bike.prototype.deal="rule"
const honda=new Bike(5000,"let's go")
console.log(`${honda.amount} is made by ${honda.ride} to do ${honda.deal}`)
```

this all the code we have explained previously.

## Prototypal Chain :→

here where we generalize this with making one function let mw show it with code :→

```javascript
//prototypal chain
Array.prototype.ayush= function () {
   console.log(`I love ${this}`)
}
let mr=["pokemon","dragin ball z"]
console.log(mr.ayush())
```

here “Array” is a object that defines all the arrays. And in this context “this” keyword show what’s the content in new “Array” we have just made named “mr”.

---

## ***class in js and Inheritance :→***

In this section we will learn about class in Javascript :→

```javascript
class Gari {
   constructor(make, model) {
      this.make = make;
      this.model = model;
   }
   start() {
      return `hello ${this.make} done by ${this.model}`;
   }
}
class Bus extends Gari {
   drive() {
      return `hello ${this.model} and ${this.make} is done`;
   }
}
let bus_46 = new Bus("bus_46", "89");
console.log(bus_46.start());
console.log(bus_46.drive());
```

---

## 2&gt;Encapsulation :→

it's the combination of variable that it's named as class symbolized as

## i&gt;Public data-field :→

```javascript
//encaptulation
// In encaptukation there must be public,private or protected data-feild
class Bus {
   // make and model are public feilds
   constructor (make,model) {
      this.make=make;
      this.model=model;
   }
   start(){
      return `${this.make} done by ${this.model}`
   }
}
const bus_46=new Bus("215","rare bus");
console.log(bus_46.start())
console.log(bus_46.make)
console.log(bus_46.model)
```

---

## ii&gt; Private data field :→

here we use private data feild which are shown by using the ***“#“ .***

more over we can’t access the private class public getter and public setter function . the function named as **getMake()** and **setMake().**

```javascript
class Airplane{
   #make;// private data-feild 
   #model;// private data-feild
   constructor(make,model) {
      this.#make=make;
      this.#model=model;
   }
   start(){
      return `nacho nachoo gao gao${this.#make} and${this.#model} `
   }
   // now can't acccess the private class outside the class. we have to make some function to use it with "setmake" and "getmake"
   getMake(){// show the output we want callled public "getter"
    return `getting...${this.#make}`
   }
   setMake(newmake){// show the output we want callled public "getter"
      this.#make=newmake;
     }
}
const royalstag= new Airplane("royalstag",69)
console.log(royalstag.getMake())
console.log(royalstag.start())
```

here are something we have to notice:→

In the **constructor function** and **setMake()** function in these function we make used “normal data-feild” we have seen then previously. this “public setter” in here we have to set the “condition” and for every data feild we make to make . we will see it while writing the code.

---

## iii&gt; Private data-feild and getter and setter :→

```javascript
class Form {
  constructor(name, age) {
    if (name.length > 0) {
      this._name = name;
    } else {
      throw new Error("error:invalid name");
    }
    if (age > 0) {
      this._age = age;
    } else {
      throw new Error("error:invalid age");
    }
  }
  //getter for name
  get name() {
    return `getting ${this._name}`;
  }
  set name(newName) {
    if (newName.length > 0) {
      this._name = newName;
    } else {
      throw new Error("eror:invalid name");
    }
  }
  get age() {
    return `getting ${this._age}`;
  }
  set age(newAge) {
    if (newAge > 0) {
      this._age = newAge;
    } else {
      throw new Error("error:invalid age!! age can't be negetive!!!");
    }
  }
}
// for error handleing
try {
   const ayush=new Form("ayush",18)
   console.log(ayush.age)
   console.log(ayush.name)
   const piyush=new Form("piyush",-18)
   console.log(piyush.name)
   console.log(piyush.age)
   // console.log(piyush.name)
   const blankName=new Form("",18)
   console.log(blankName.age)
   console.log(blankName.name)

} catch (error) {
   console.error(error.message)
}
```

---

## iv&gt; here we combine the private data field and getter and setter :→

```javascript
/conbination of data input feild and getter and setter
class Form{
   #name;
   constructor(newName){
       this.#name=newName;
   }
   getName(){// making a gettter methos  that job is to give name
      return `${this.#name} is geting name`
   }
   
}
const ayush=new Form("ayush");
console.log(ayush.getName())
```

---

# 3&gt;polymorphism:→

```javascript
//polymorphism means here can be many object has same methos and they can show poly(many different) result
class Shape {
  constructor(name) {
    this.name = name;
  }
  draw() {
    return `draw a generic shape!!!`;
  }
}
//making circle class
class Circle extends Shape {
  constructor(radius) {
    super("Circle");
    this.radius = radius;
  }
  draw() {
    return `${this.radius} is the radius of the circle.`;
  }
}

//making rectangle class
class Rectangle extends Shape {
  constructor(width, length) {
    super("Rectangle"); // inerhit the main class contructor function
    this.width = width;
    this.length = length;
  }
  draw() {
    return `width is ${this.width}and length is ${this.length} and ${
      this.width + this.length
    } is the perimeter of the rectangle.`;
  }
}

const circle = new Circle(5);
console.log(circle.draw());

const rectangle = new Rectangle(5, 9);
console.log(rectangle.draw());
```

note :→ without <mark> “super(“circle”)”</mark> the parent class constructor’s name will not initialized. that’s why we have to use it.

---

so there is a concept as <mark>“</mark>***<mark>duck-typing</mark>***<mark>“</mark>

by which we can implement the concept of **<mark>“polymorphism”</mark>**

so as of let’s ignore this cz it’s actually is in “typescript” and “java”.

---

# 4&gt;abstraction:→

it’s actually the process of hiding the complex process and make user know the usefull thing for the process.

```javascript
//polymorphism means here can be many object has same methos and they can show poly(many different) result
class Shape {
  constructor(name) {
    this.name = name;
  }
  draw() {
    return `draw a generic shape!!!`;
  }
}
//making circle class
class Circle extends Shape {
  constructor(radius) {
    super("Circle");
    this.radius = radius;
  }
  draw() {
    return `${this.radius} is the radius of the circle.`;
  }
}

//making rectangle class
class Rectangle extends Shape {
  constructor(width, length) {
    super("Rectangle"); // inerhit the main class contructor function
    this.width = width;
    this.length = length;
  }
  draw() {
    return `width is ${this.width}and length is ${this.length} and ${
      this.width + this.length
    } is the perimeter of the rectangle.`;
  }
}

const circle = new Circle(5);
console.log(circle.draw());

const rectangle = new Rectangle(5, 9);
console.log(rectangle.draw());
```

draw() is the example abstraction.

---

# **Summary of Mastering JavaScript OOP**

In this comprehensive guide, we explored the fundamental concepts of Object-Oriented Programming (OOP) in JavaScript. Here's a recap of the key topics covered:

---

1. **JavaScript: OOP vs. Prototype-Based**  
    JavaScript, at its core, is prototype-based but incorporates OOP principles for developers' convenience. Understanding the **prototype chain** is crucial for mastering JavaScript OOP.
    
    * **Prototype Chain**: Using `__proto__`, `Object.setPrototypeOf()`, and `Object.getPrototypeOf()` to manipulate object inheritance.
        
    * **Functional Constructors**: A practical approach to creating objects and extending them using `.prototype`.
        

---

2. **Core OOP Concepts**:
    
    * **Classes and Inheritance**: Creating blueprints (`class`) and extending functionality using `extends` and `super`.
        
    * **Encapsulation**: Protecting data with public and private fields (`#field`) and controlling access via getters and setters.
        
    * **Polymorphism**: Overriding methods like `draw()` to create varied behaviors for different objects, e.g., `Circle` and `Rectangle`.
        
    * **Abstraction**: Hiding implementation details and exposing only the essential functionalities through methods.
        

---

3. **Code Examples**:  
    Throughout the blog, we used practical examples to demonstrate OOP principles:
    
    * Creating and linking prototypes.
        
    * Functional constructors with `.prototype`.
        
    * Classes for real-world objects like `Car`, `Fruit`, `Bus`, `Shape`, `Circle`, and `Rectangle`.
        

---

4. **Real-Life Applications**:
    
    * **Prototypes**: Ideal for memory-efficient object sharing.
        
    * **Classes**: Streamlined object-oriented structures.
        
    * **Encapsulation**: Data protection and validation.
        
    * **Polymorphism**: Dynamic and reusable behavior for diverse object types.
        

---

### **Final Thoughts**

This guide provided a solid foundation in JavaScript OOP, blending practical examples with theoretical concepts. Mastering these principles will enable you to write cleaner, more modular, and scalable code.

Now that you've conquered JavaScript OOP, you're ready for the next step: exploring the **Document Object Model (DOM)** to build interactive web applications.

Keep coding and learning! 🚀  
— **AyushtheBatman** (Full Stack Developer)