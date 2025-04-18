---
title: "JavaScript Basics: Mastering Variables, Loops, and Arrays for Beginners"
seoTitle: "JavaScript Foundations: Learn Variables, Loops, and Arrays Easily"
seoDescription: "Build your JavaScript foundation with this beginner's guide! Master essential programming concepts like variables, loops, and arrays through problems"
datePublished: Sun Nov 24 2024 03:18:29 GMT+0000 (Coordinated Universal Time)
cuid: cm3v14qyy002n09mhee8f2nif
slug: javascript-basics-mastering-variables-loops-and-arrays-for-beginners
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1732418268496/753158c1-ca56-47fc-9b7e-0d98ccd4c4aa.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1732423622361/a78fd3cd-9e69-4c29-bdb8-8833f4f96d6e.png
tags: tutorial, js, programming, javascript, typescript, functional-programming

---

**Description:**  
Start your coding journey with this beginner-friendly guide to JavaScript. Explore the foundational concepts of programming, including variables, loops, and arrays, explained with simple examples and practical exercises. Perfect for those new to coding, this guide will help you build a strong base for web development and beyond.

---

# 1&gt; Datatype and var let and const :-&gt;

## i&gt; Data-type: -&gt;

a&gt; string(alphabet)

b&gt;number(1...big n)

c&gt;Boolean(true and false )

d&gt;bigint( bigger number)

e&gt;undefined( there is something that is not empty)

f&gt;null ( there is something and that's empty)

g&gt;object (collection of diff datatype)

h&gt;symbol(emoji)

## ii&gt; var,let and const :→

a&gt; var has global scope and can be changed

b&gt; let has local scope and can be changed is we want

c&gt;const has local scope and the value don't changed.

---

# 2&gt;operation in JavaScript: -&gt;

## a&gt;Arithmetic operator: -&gt;

i&gt;addition \[+\]

ii&gt;subtraction \[-\]

iii&gt;multi-plication \[\*\]

iv&gt;power (\*\*\*) =\[2\* 3\*3\]

v&gt;modulus (give remainder):→ \[%\]

## b&gt;comparison operator :-&gt;

( give answer in Boolean )

i&gt; "&lt;"/"&lt;=" =&gt;ezpz

ii&gt; "&gt;"/"&gt;=" =&gt; ezpz

iii&gt; "==" =&gt; check that both are same or not

iv&gt; "===" =&gt; strictly check that.

## c&gt; logical operator :

i&gt; && =&gt; both condition must be satisfied

ii&gt; || =&gt; anyone condition must be true

iii&gt; != =&gt; not equal to

## d&gt; assign operator :-&gt;

i&gt; a+=b =&gt; a=a+b;

---

# 3&gt; primitive data-type :

i&gt;string

ii&gt;Boolean

ii&gt;number

iv&gt;null

v&gt;undefined

vi&gt;symbol

a&gt; by "typeof()" we can get the title of the data.

b&gt; let a=10; =&gt;number let b= new Number(10) =&gt;object

c&gt; let a ; =&gt; a exist but a is not here so it's "undefined";  
d&gt; let a = undefined =&gt; we have to mention

e&gt; string interpolation :-&gt; \`${}\`

f&gt; symbol give the unique name .. that can't be same

g&gt; non-primitive data type:-&gt;

i&gt; object

ii&gt; array

---

# 4&gt;Object and Array :-&gt;

### making a object…

→let information = { firstname :ayush;

is logged in :true;

last-name:basak; }

a&gt; accessing the object :→ log(information.firstname); =&gt; ayush

b&gt; we can add more element in the object

---

5&gt;conditionals :-&gt;

if and else ... and "if" clock executes then part of the code will be executed and "else" block will be executed

ex:-&gt;

`if(conditions){`

`console.log(something)`

`}`

`else{`

`console.log(something2)`

`}`

here is a pictorial presentation to understand it better

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1731840946021/f4a99e0d-8fcd-4392-8395-c44a8834d9c7.png align="center")

---

# 6&gt;arrays :-&gt;

a&gt; making the array :-&gt; let cities = \["London","Kolkata","Paris"\];

b&gt; accessing the array :-&gt; log(cities\[0\]) → london

note :-&gt; array start from 0 to (n-1)

c&gt; push( add the element 1st to last )

d&gt; pop ( reduce the array last to 1st )

e&gt; soft copy ( if we change in variable and store the variable value in another spot then the another spot’s value will not change and it’s generally seen in primitive data type.{number,string etc} )

f&gt; hard copy \[...array\]=&gt; {rest and spread operator} =&gt; {<mark>hard copy means if we change the actual array then the “another spot” where we have store the value of array is saved</mark>

g&gt; concat(arrayname)=» {adding two array}

---

# 8&gt; loops

a&gt; introduction :-&gt;

there is there steps

i&gt; they are :-&gt;

1&gt; initialization 2&gt; condition 3&gt; set of instruction

they loop every time, until they get the termination to stop it. get the rest part of the code

b&gt; they are some loops we will try run and learn from it

here is a picture to better understand the “loops “ better

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1731841028157/f0896aae-23dd-4642-91d4-7bb4b14d5717.png align="center")

---

### a&gt; do-while :→

syntax of do-while loop :→

```javascript
// do while loop 
do {
  // prompt(``)
} while (condition);
```

when we are sure that at least one time ...

To practice the loop we have designed diff type of exercises :-&gt;

<mark>exercise-1 : write a program with using the "do-while" loop and make a "prompt" [ see on MDN to know more about it ] &amp; the prompt should say "write the name of the superheroes you want to meet and write "stop" to stop it " and here we have to show the list of the superheroes</mark>

```javascript
// do while loop 
let herocollection=[];
// herocollection is array. 
// that's why the promt came again and again.
let hero="";
// this is the input feild 
do {
  hero= prompt(`write the name of the superheroes you want to meet and write "stop" to stop it`)
  // here the given name will be saved at "hero"
  if (hero!="stop") {// if hero is not =  to stop then next block of the code will be run 
    herocollection.push(hero)
    // herocollection is empty array  
    // In that array we will push (add from 1 to last )
    // and that will make herocollection aray that is new
  }
} while (hero!="stop");
// untill we white "stop" promt will not stop
```

---

<mark>exercise-2 : write a "do-while" loop and add " 1 to 3 " and store in a variable named "TOTAL"</mark>

```javascript
//exercise-2 : write a "do-while" loop and add " 1 to 3 " and store in a variable named "TOTAL"
let k=0;
let total=0;
do {
  total=total+k;
  k++;
  console.log(total)
  
} while (k<=3);
```

### b&gt; while loop : -&gt;

syntax of while loop :→

```javascript
// while loop prblms and try to understand it :-> 
// sytax of while 
while (condition) {
  here the set of instruction will run 
}
```

<mark>In “While” loop we have to first check the conditon then run it not like do-while</mark>

when we know the condition then we have to use while loop

To practice the loop we have designed diff type of exercises :-&gt;

<mark>exercise-1: add 1 to 5 with the help of "while" loop</mark>

```javascript
// while loop prblms and try to understand it :-> 
// sytax of while 
let sum=0;
let i=0;
//  intially let's assume the sum and i is 0;
//  here we assume that i will loop and sum will store the values 
while (i<=5) {
  sum=sum+i;
  i++;
}
console.log(sum);
```

<mark>exercise-2: store 5 to 1 in the array named "series" with the help of "while" loop</mark>

```javascript
//exercse:2 -> 
let series=[];
let j=1;
while (j<5) {
  series[j]=series.push(j)
  j++;

}
console.log(series)
```

---

### c&gt; for loop : -&gt;

the syntax of the “ for loop “ with respect to “arrays”

```javascript
for (let index = 0; index < array.length; index++) {
  const element = array[index];
  
}
```

syntax of “ for loop “ in more generalised version : →

```javascript
for (intial condition; index < termination condition; index++) {
 // things we want to do 
  
}
```

when we know how many time the code will run then we use this loop

To practice the loop we have designed diff type of exercises :-&gt;

<mark>exercise-1 :-&gt; name a array named " numbers " and store values like = [3,6,3] and multiply with ( 3 ) and then save those value in another array named " multiples"</mark>

```javascript
//exercise-1 :-> name a array named " numbers " and store values like = [3,6,3] and multiply with ( 3 ) and then save those value in another array named " multiples"
let numbers =[3,6,3];
let multiple =[];
for (let index = 0; index < numbers.length; index++) {
  // above line is used for going through the whole array 
  const element = numbers[index];
  multipleX=element*3;
  multiple.push(multipleX);
  // console.log(element);
  console.log(multiple);
}
```

<mark>excercise-2:-&gt; there is array named superhero where we have saved as ["batman","superman","ironman"] and so the task to make the every name of the superhero a different array " antiheros "</mark>

```javascript
//excercise-2:-> there is array named superhero where we have saved as ["batman","superman","ironman"] and so the task to make the every name of the superhero a different array " antiheros "
let superheros=["batman","superman","ironman","venom"];
let antihero=[];
for (let index = 0; index < superheros.length; index++) {
  const element = superheros[index];
  antihero.push(element);
console.log(`the original arrays is ${superheros}`)
  console.log(`the changed  arrays is ${antihero}`)

}
```

---

## And we will try to 10 problems on our own with some additional knowledge and here we will cover all the loops in JavaScript :→

---

### exercise-1:-&gt; Use "for" loop there is a array named “superheros”=\["Batman","Ironman","Thor","Venom" \] and the job is when we will see \[ "Thor" \] we will simply skip it and we will only print the array before \["Thor"\]. hint-1: use break to break the loop

```javascript
// Use "for" loop there is a array named ["Batman","Ironman","Thor","Venom" ] and the job is when we will see [ "Thor" ] we will simply skip it and we will only print the array before ["Thor"]. hint-1: use break to break the loop
let superheros=["Batman","Ironman","Thor","Venom" ]

let ayush=[];

for (let index = 0; index < superheros.length; index++) {
  const element = superheros[index];
  if (element==="Thor") {
    break;
  } 
    ayush.push(element);
}
console.log(superheros);
console.log(ayush)
```

---

### exercise-2:-&gt; Use "for" loop there is a array named \[ "Batman","Ironman","Thor","Venom" \] and the job is when we will see \[ "Thor" \] we will simply skip it and we will print the array without\["Thor"\].

```javascript
// Use "for" loop there is a array named ["Batman","Ironman","Thor","Venom" ] and the job is when we will see [ "Thor" ] we will simply skip it and we will only print the array before ["Thor"]. hint-1: use break to break the loop
let superheros=["Batman","Ironman","Thor","Venom" ]

let ayush=[];

for (let index = 0; index < superheros.length; index++) {
  const element = superheros[index];
  if (element==="Thor") {
    // break; <- leavr the loop at that point 
    continue;// skip the "condition" and print the rest of th part 
  } 
    ayush.push(element);
}
console.log(superheros);
console.log(ayush)
```

---

### exercise-3:-&gt; Use "for-of" loop and go-through the array where it's stored that \[1,2,3,4,5\] and we have to make the array that has numbers before "4" and the array is called as "small\_nums".

---

### note :→

## <mark>what is “for of " loop?</mark>

---

### here is the syntax of it :→

```javascript
for (variable of iterable) {
  // Code to execute for each element
// variable :-> name of the new thing 
// iterable :-> 
}
```

---

solution :→

```javascript
let numbers=[1,2,3,4,5]
let ayush=[];
for(let ez of numbers) {
  if (ez===4) {
    break;
  } 
    ayush.push(ez);
  }
console.log(ayush)
```

exercise-4:-&gt; Use "for-of" loop and go-through the array where it has stored \[1,2,3,4,5\] and we have to make the array that has numbers except "4" and the array is called as "prefered\_nums".

```javascript
let numbers=[1,2,3,4,5]
let ayush=[];
for(let ez of numbers) {
  if (ez===4) {
    // break;
    continue;
  } 
    ayush.push(ez);
  }
console.log(ayush)
```

exercise-5:-&gt; Use "for-in" loop and loop through an object named -&gt; "city" and stop at "London" and make an object named "new\_citi".

let Citi={ "New York":100k;

"Canada":150k;

"Pakistan":500k;

"London":300k; }

---

### understanding the “for-in” loop

```javascript
for (let key in object) {
  // Code to execute for each key
}
// for in always used in "objects"
// for of always used for "arrays"
```

---

solution of the problem :→

```javascript
let Citi={ 

"New York":"100k",

"Canada":"150k",

"Pakistan":"500k",

"London":"300k" }
let new_city={

}
for (const ez in Citi) {
  // here in the object the key act as the index in array 
  //
  if (ez==="London") {
    break;
    // this will the break the loop on the condition 
    
  }
  new_city[ez]=Citi[ez];
}
console.log(new_city);
```

---

## understanding the “for-each” loop :→

```javascript
array.forEach(function(element, index, array) {
  // Code to execute for each element
});
// using the normal function 
//or
array.forEach((element, index, array)=>{
  // Code to execute for each element
});
//using the array function
```

---

exercise-7 :→ Use "for-each" loop there is array named number=\[1,2,3,4,5,6,7,8\] and the condition is whenever we reach to \[7\]. we have print the rest of the cities in the another array name is ”sm”.

---

the solution of the problem :→

```javascript
let number = [1, 2, 3, 4, 5, 6, 7, 8];
let sm = [];

number.forEach(ez => {
  if (ez !== 7) { 
    sm.push(ez);
  }
});

console.log(sm);
```

exercise-8: → Use “for” loop and there is an array named numbers that has \[1,2,3,4,5,6,7\] so stop at “5” and multiply the rest of the number with “7“ and save that in the new array name “qt\_num” and store the numbers in that.

```javascript
let num=[1,2,3,4,5,6,7]
let qt_num=[];

for (let index = 0; index < num.length; index++) {
  if (num[index]=== 5) {
    continue;
  } 

 qt_num.push(num[index])
}
console.log(qt_num)
```

---

## 9&gt; function, arrow function and this context :→

### function :→ In remote there is multiple buttons that has different purpose in same way there is function that has specific way to a assigned task.

example :→ write a function that can 2 number

```javascript
function sumnum(a,b) {
  return a+b;
  }
let ans=sumnum(2,5);
console.log(ans);
```

---

## Arrow function :→

### In ES6 they introduce the arrow function it’s more easy to use and more efficient let me show the syntax for it :→

```javascript
sumnum=(a,b)=>{
  return a+b;
  }
let ans=sumnum(2,5);
console.log(ans);
```

I have writen it for same function with arrow funtion to for ez of understanding.

---

## THIS context :→

### 1&gt; “THIS” is a keyword for objects that used for <mark>object’s reference</mark> and it only can be used for a <mark>context of “object” only.</mark>

### 2&gt; we cannot use “<mark>arrow function</mark>“ to use “THIS” keyword and we have to use “<mark>regular function</mark>”

let me show that with example :→

```javascript
const ayush ={
  name:`babai`,
  age:18,
  ph_number:999999,
  fav_foood:`biriyani`,
  fav_place:`germany`,
  togo:function tocome() {
    console.log(`${ayush.name} love to eat ${ayush.fav_place}`);}}
ayush.togo();
```

firstly guess the output and then see the output :→

here “ayush“ is the object name . and togo is a function that use “string interpolation”.

---

### now as reference we will use “this” key-word :→

means where we have used ayush object to exchange that reference we will use “ this “ key-word here is the example:→

```javascript
const ayush ={
  name:`babai`,
  age:18,
  ph_number:999999,
  fav_foood:`biriyani`,
  fav_place:`germany`,
  togo:function tocome() {
    console.log(`${this.name} love to eat ${this.fav_place}`);
    }
}
ayush.togo();
```

here we will also get the same output .

try to copy paste and try to see that on your own and execute.

3&gt; for multiple object and multiple this :→

```javascript
const ayush ={
  name:`babai`,
  age:18,
  ph_number:999999,
  fav_foood:`biriyani`,
  fav_place:`germany`,
  togo:function tocome() {
    console.log(`${this.name} love to eat ${this.fav_place}`);
    }

}
const piyush ={
  name:`pagal`,
  age:18,
  ph_number:999999,
  fav_foood:`kinderjoy`,
  fav_place:`NYC`,
  togo:function tocome() {
    console.log(`${this.name} love to eat ${this.fav_place}`);
    }
}
ayush.togo();
piyush.togo();
```

here is the output :→

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1732947790687/b0d10910-02bd-4b0a-a4ff-05937802809e.png align="center")

---

## 10&gt; Higher order function and Nested function :→

```javascript
//nested function :->
function ayush(){
  console.log(`hi bhai`);
  function piyush(){
    console.log(`how are you?`);
  }
  piyush();// this will run
}
ayush();
piyush();// this will not be executed 
// cz function will only executed only in local scope
```

### when the function is in another function it is called <mark>“nested function”</mark>

---

## Higher Order Function (H.O.F):→

def :→ when a function take “function” as <mark>“argument “</mark> and <mark>return “ function” as “output“</mark>

### more hof we will learn it on “call backs” and “settimeout“ later .

now we will see some other example:→

```javascript
function addnum(func){
  return function (value){
    return value+func;
  }
}
const ayush=addnum(2);//2+0
console.log(ayush(5));//2+5
```

---

# **Summary: Building a Strong Foundation in JavaScript**

Embarking on your JavaScript journey can feel overwhelming, but this beginner-friendly guide has broken down complex concepts into easy-to-digest pieces. From understanding the origins of JavaScript and its transformation through V8, Node.js, Bun, and Deno to unraveling the behind-the-scenes magic of `console.log("Hello World!")`, you’ve taken your first steps toward mastery.

Key topics covered include:

* **Data Types**: A thorough exploration of primitive (string, number, boolean, etc.) and non-primitive (objects and arrays) data types, alongside the nuances of `var`, `let`, and `const`.
    
* **Operations and Conditionals**: Understanding arithmetic, logical, and comparison operators to shape your code logic effectively.
    
* **Loops**: Practical exercises for mastering `for`, `while`, `do-while`, `for-in`, and `for-of` loops, helping you iterate over data and perform complex operations.
    
* **Functions and Arrow Functions**: Learning the syntax, benefits, and use cases of regular and arrow functions, along with the importance of the `this` keyword in object references.
    
* **Higher-Order and Nested Functions**: Introducing the concepts of functions that take or return other functions for advanced code structuring.
    

Through hands-on examples and exercises, you’ve built confidence in manipulating arrays, objects, and loops, and you’ve laid the groundwork for tackling JavaScript’s advanced features like object-oriented programming (OOP).

JavaScript is more than a language; it's a gateway to dynamic web development and modern-day programming challenges. Keep exploring, experimenting, and practicing. The next stop? JavaScript OOPs!

*By Ayushthebatman(Full Stack Web Developer)*