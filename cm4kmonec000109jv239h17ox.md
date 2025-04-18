---
title: "TypeScript Mastery: The Ultimate Guide to Building Robust JavaScript Applications"
seoTitle: "TypeScript Mastery: The Ultimate Guide to Building Robust JavaScript"
seoDescription: "Unlock the power of TypeScript with our comprehensive guide. Learn how to enhance your JavaScript development, improve code quality, and build scalable apps"
datePublished: Thu Dec 12 2024 01:16:04 GMT+0000 (Coordinated Universal Time)
cuid: cm4kmonec000109jv239h17ox
slug: typescript-mastery-the-ultimate-guide-to-building-robust-javascript-applications
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1733966426995/15644c03-772d-4278-871e-41d23f26f3ef.png
tags: software-development, programming, javascript, typescript, functional-programming, software-engineering

---

Description:→ Unlock the power of TypeScript with our comprehensive guide. Learn how to enhance your JavaScript development, improve code quality, and build scalable applications with strong type checking and modern web development techniques.

---

## 1&gt;why do we need “TypeScript” when we have “JavaScript”?

So, the answer we will in after sometimes firstly we will install the “TypeScript” in our system and then we will answer this. So, it will be a fun journey so let’s start :→

## a&gt; Installation of “TypeScript” :→

so there is couple of way we can do this :→

**i&gt;**[**click on this to install "TypeScript"**](https://www.npmjs.com/package/typescript)

**<mark>or</mark>**

```bash
npm i -g typescript
```

use this command on the “vs code” terminal. And congratulation! **<mark>TypeScript</mark>** is in your system. To check that you have to write

```bash
tsc -v
```

by which we can get the version of the “TypeScript”. And if it’s showing then …. yess yesss yessss!!!… installation is done . :-)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1733973949557/ba3cd5f0-ace1-4a61-8f8a-594d8c7eb6e6.png align="center")

---

## 2&gt; Now we have to move on to 2nd part that’s compile “TypeScript”

For that we have to write another command that we also have to execute on “terminal” .

```bash
tsc
```

“tsc” is the only compiler that will help to compile the “TypeScript” code to “JavaScript” . And that will be again “byte code” means all “0” and “1”.

---

## 3&gt; How “TypeScript” code will run after compilation?

so there 2 analogy to use “TypeScript”

## a&gt;without making the folder structure.

i&gt; write your “ts” code.

ii&gt; compile it to “js”.

iii&gt;make a html file attach the the “js” code .

iv&gt; and see the out put on console section in the inspect part of broswer.

## b&gt;with folder structure.

there process will be same but here we have to mention the outdir(output location)\[js part\] and rootdir(input section)\[ts part\] in “tsconfig section”.

now here come the next question “ how to make the tsconfig part?” so let’s answer it too.

---

## 4&gt;how to make the tsconfig. part in “TypeScript?

```bash
tsc -init
```

this will generate tsconfig where we can set-up the “rootdir” and”outdir”.If we want to write the the adress we can make sure the input and output part of the “project”.<mark>Now the question is every time we make any change in “ts” file we have to restart the “ts” with “tsc” again and again. we will answer it in this section.</mark>

---

## 5&gt;how to watch “ts” changes in the project ?

```bash
tsc -w
```

we have to use in “terminal” in “vs code” and that’s enough. if we change anything in “ts”, we will the changes in “js” file and console(browser) too.

---

now the question is when we have “JavaScript” then why we are trying to go through the “new language” named “TypeScript”. here is why →

---

## 6&gt;why we need “TypeScript” ?

<mark>i&gt;”JavaScript” is</mark> **<mark>dynamically typed</mark>** **<mark>language</mark>**<mark>. “TypeScript” </mark> **<mark>Statically typed language.</mark>**

note :→ now the question is :→ what is “**Dynamically typed** **language” and “Statically typed language” ?**

**“S**tatically ty**ped** language\*\*” means it checks the “types” of variable during the compilation of code.\*\*

**“Dynamically typed** **language” means it checks during the “run-time” that’s the “execution of the code”.**

<mark>ii&gt;”JavaScript” is </mark> **<mark>interpreted language</mark>** <mark>and “TypeScript” is </mark> **<mark>compiled language.</mark>**

note :→ now the question is :→ what is “**compiled language” and “interpreted language” ?**

“**compiled language” means it get complied to machine code then execute on the computer.**

**“interpreted language” means it will be get compiled as it runs(line by line as execute)**

that the theoretical reason of we should use “TypeScript”.

now let’s under stand this by code.

here we will write the same code see the benifits of it .

```javascript
let a=20;// started as number 
a="ayush";// changed to string
console.log(a);// ayush
```

here a is “number” at first and then a became “string” this can make error in the program . let’s asuume in “auth” project we wanna take username only as “string”. when we specific type we us this.

```typescript
let a = 20; // started as number
a="ayush"
console.log(a); // error
```

this same code will give us error!!!.. let’s see that too.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1734024541238/e5e203a9-3a6f-43e8-aaa3-b2894df76fa2.png align="center")

---

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1734024594546/8cc91e2a-5a26-487e-bfe6-9132e169a622.png align="center")

---

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1734024628874/3ceb664c-bd19-4ee5-a6a5-a1772fe7eb9f.png align="center")

---

here as this picture we have shown the “Error” we try to use a as “number” and later try to make “string” but “ts“ will nit do it. And also give me the error. here is the right code

```typescript
let a :number = 20; // started as number
console.log(a); // 20
```

---

here the js file after compilation it’s like this code :→

```javascript
"use strict";
let a = 20; // started as number
console.log(a); // 20
```

---

so. i guess in was the enough motivation to start our journey with **<mark>TypeScript the another main reason is it give us error while writing the code not in the run_time stage as it’s not a “interpreted language” as “JavaScript” so it make more robust system and more efficient all in all.</mark>**

---

## 7&gt; Is TypeScript new language ?

short answer : NO

long answer : TypeScript is superset of “JavaScript” . It has some extra properties that make the “js” code more better and robust and on this section we are gonna see those features.

---

---

# let’s deep dive into “TypeScript”:→

## 1&gt;introduction to basic types: →

so there is 2 type of data type in the "programming” part.

a&gt; **primitive data-type** :→ number, string , boolean.

b&gt;**no-primitive data-type** :→ array, object etc.

now here is the question is :→ **what’s primitive data-type and non-primitive or reference data-type ?**

**primitive is data-type that**

**1&gt; cannot be broken further and represent a simple data-type.**

**2&gt;And has a fixed type too.**

**3**\&gt; \*\*primitive data-type is “<mark>addressed by value</mark>” means if we copy the variable in another variable .It give actual copy of the variable(\*\*separate **copy), it give us the actual value of the variable , js/ts store the primitive data type in “<mark>call stack</mark>”. And if we changes the copied variable (another one). then only the copied variable will be changed. But the original value will be unchanged.**

```typescript
let original_num:number=12;
let copied_num:number=original_num;
copied_num=13;
console.log(`copied_num is ${copied_num} and original_num is ${original_num}`);
// adress by value
```

example:→number ,string ,boolean etc.

---

**reference / non-primitive is data-type that**

**1&gt; can b**e broken **further cz it’s <mark>mixture</mark> of one or many data-types.**

example : object ,arrays etc.

```typescript
let course_obj={
  first_name:"piyush",//string
  age:12,// number
  is_paid:true // boolean
}
```

**2&gt;non-primitive data-type is “<mark>addressed by address</mark>” means if we copy the variable in another variable .it doesn’t give actual (separate)copy of the variable , it give the address of the variable to us, js/ts store the non-primitive data type in “<mark>heap memory</mark>” . And if we changes the copied variable (another one). then only the copied variable will be changed. And the original var will be also changed.**

---

# 1&gt;primitive data-type:→

data-types are :→

a&gt;number

b&gt;string

3&gt;boolean

---

# 2&gt;Array:→

as normal “js” but “ts” define the type as we assign the values of “array”.

```typescript
let ayush = [1, 2, "ayush", true];
console.log(ayush);
let piyush = [1, 22, 3];
console.log(piyush);
```

---

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1734247708053/c8ee7d1e-27bc-45f0-b475-a0e174941af8.png align="center")

---

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1734247767728/04e53cb2-ea44-41d8-8be2-cd0db62bb868.png align="center")

---

# 3&gt;Tuples:→

A **tuple** is a typed array with pre-defined length and types for each index.

```typescript
let ayush: [string, number] = ["batman", 22];
let piyush: [string, number] = ["ironman", 23];
//tuple
```

---

# 4&gt;E-num (e-numeration):→

An **e-num** is a special "class" that represents a group of constants (unchangeable variables).

```typescript
enum StatusCodes {
  NotFound = 404,
  Success = 200,
  Accepted = 202,
  BadRequest = 400
}
console.log(StatusCodes.NotFound);
console.log(StatusCodes.Success);
```

---

# 5&gt;Any ,Unknown ,Void, null ,undefined, never :→

## a&gt;any:→

**“Any”** :→if we don’t specify the type of the variable in my program then it will automatically set the value to any. Then we can assign any value to the variable that’s means if we use “<mark>any</mark>” keyword then it will just “turn off” …. “TypeScript”.. cz we can do the same task with “JavaScript”.

```typescript
let ayush;
ayush = 12;
ayush = "batman";
```

---

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1734258535648/66016e70-e599-4231-bda1-be59903ff86d.png align="center")

if we don’t mention any type then by default variable’s type will be “any”.

## note:→don’t use “<mark>any</mark>” keyword if u wanna use “<mark>TypeScript</mark>”.

---

## b&gt;unknow:→

```typescript
let ayush: unknown;
ayush = 12;
ayush = "batman";
if (typeof ayush === "string") {
  console.log(ayush.toUpperCase);
}
```

difference between “any” and “unknow” is later we can assign the value to it. and use it by checking the type.

---

## c&gt;void:→

if a function doesnot return any thing, we have to use “void” keyword another wise we have to specify the return type of the function.

```typescript
function ayush(a: number): void {
  console.log((a = a + 10));
}
let piyush = ayush(10);
```

---

if the function is returning anything then we have to mention it’s type like:→

```typescript
function ayush(a: number): number {
  return((a = a + 10));
}
let piyush = ayush(10);
console.log(piyush);
```

---

At that point we have to use “return keyword”. otherwise we will get error.

---

now the question is :→ why “void” function is being used?

the reason is :→ ***it is used to “console.log” , “modifying the states” , “triggering the async function”.***

---

## d&gt;null :→

let’s assume we are trying to find a name in database of millions. And if we can’t find then simply we will get “null” as result. that means we can’t further add or assign the value in the variable.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1734274303566/96f07c56-39fe-416f-a3d6-eeec22c2c3ca.png align="center")

---

## e&gt;undefined :→

```typescript
let a: undefined;
```

---

## f&gt;never :→

```typescript
function ayush(): never {
  while (true) {}
}
ayush();
```

while(true) =&gt; will just start infinite loop. and if run then the programm will not stop if we want our program or function doesn’t show anything. We will use “never” keyword.

---

# 6&gt;Type inference and Type annotation :→

```typescript
let a=12;
```

# Type inference:→

if we write the above code and “typescript” auto-matically detect that a is “number”. that’s called as “Type inference”.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1734276006154/c420d78e-a150-4a4d-8843-c14a3573fabd.png align="center")

---

# Type annotation :→

```typescript
let b: number;
b = 13;
```

when we mention the “type” of the variable on our own that’s “Type annotation”.

---

# 7&gt; Type interfaces and type alias :→

```typescript
interface MOmo {
  name: string;
  password: string;
  age: number;
}
function ayush(abcd: MOmo) {
  return `${abcd.name} is ${abcd.age}years old and his password is : ${abcd.password}`;
}
let batman = ayush({ name: "ayush", password: "ayush123", age: 12 });
console.log(batman);
```

interface is a syntactical contract that defines the structure and properties of the “object”.

see the error for better understanding.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1734277006052/71eea389-c4a4-4409-a4d0-15edf1c4933b.png align="center")

## a&gt;extending interfaces :→

using “extends” keyword we can add more “property” by which we can add more properties to a particular object i.e. “MOmo2” .

in the functional parameter we are passing adcd1 that has same property as “MOmo2“ and that’s what interface and extending interfaces do.

```typescript
interface MOmo1 {
  name: string;
  password: string;
  age: number;
}
interface MOmo2 extends MOmo1{
  isEating: boolean;
}
function piyush(abcd1: MOmo2) {
  return `${abcd1.name} is ${abcd1.age}years old and his password is : ${abcd1.password} and "${abcd1.isEating}" means you are having momo`;
}
let catwoman = piyush({ name: "piyush", password: "piyush123", age: 18, isEating:true});
console.log(catwoman);
```

here is the error part to understand it more better.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1734278414838/db64bb66-e52c-4c8c-a973-91b99bf9cb7b.png align="center")

---

## b&gt; Type Alias :→

it is used to make custom “types” in the language.

```typescript
type numbor = string | number;
let password: numbor = "ayush";
password = 123;
console.log(password);
```

---

## c&gt;intersection of “types” :→

```typescript
type User = {
  name: string;
  password: number;
};
type admin = User & {
  getdetails: boolean;
};
function Ayussh(batman: admin) {
  return `${batman.name} have a password is: ${batman.password} and if ${batman.getdetails}is true then you are eating momo`;
}
let piyush = Ayussh({ name: "Batman", password: 123, getdetails: true });
console.log(piyush);
```

here with a “&“ sign we can do “intersection of types” and here admin type is a great example of it. Intersection is used to extended the types.

---

# 8&gt;Class and object (in ts):→

## a&gt;Making the Class :→

```typescript
class User {
  name = "ayush";
  age = 18;
  isfat = true;
}
let newUser1 = new User();
```

---

here you can see the output.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1734358415581/0ddd4381-59f0-4a21-80b8-2226f71ac21f.png align="center")

---

## b&gt;Constructors :→

Class constructors are very similar to functions. In this class the we don’t have function use “Constructors function”.

example:→ the car factory there is many machine that make car, here the car machine is the “Constructors Function” .If we make class without

```typescript
class User {
  constructor(public name: string, public age: number, public isFat: boolean) {}
}
let ayush = new User("ayush", 18, true);
let piyush = new User("piyush", 19, false);
```

---

output:→

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1734399465710/c25e4cfe-f554-4208-bfc2-158c3be0696d.png align="center")