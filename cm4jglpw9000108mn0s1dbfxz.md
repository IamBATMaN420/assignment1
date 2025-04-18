---
title: "Mastering Async JavaScript: A Comprehensive Guide to Promises, Callbacks, and Async/Await"
seoTitle: "Mastering Async JavaScript: A Comprehensive Guide to Promises,callback"
datePublished: Wed Dec 11 2024 05:38:03 GMT+0000 (Coordinated Universal Time)
cuid: cm4jglpw9000108mn0s1dbfxz
slug: mastering-async-javascript-a-comprehensive-guide-to-promises-callbacks-and-asyncawait
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1733895284722/739446a8-11cd-46f4-9821-3d5964fa5862.webp
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1733895376148/3d042e8f-8da3-4dff-ae7b-09adf0229732.webp
tags: javascript, asynchronous, promises, async, asynchronous-javascript

---

Description:→Unlock the power of asynchronous JavaScript with this guide. Learn how to use callbacks, promises, and async/await to build efficient, responsive web applications. Perfect for developers of all levels

---

# 1&gt;Asynchronous JavaScript with Event Loop :→

so we will see it in 2 forms to understand the **async nature of “JavaScript**”.

## **1&gt;Pictorial represent :→**

## a&gt; why we need “async nature of js”?

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1733899397392/6ac1b60f-bb1f-4a62-bd34-96f7dcdfbf22.png align="center")

---

## 2&gt;How the “ASYNC JS“ works with “Event Loop” ?

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1733899620182/f3f03a26-449a-4483-a00c-6906e6920349.png align="center")

## 2&gt; By code :→

so 1st we start with “time functions” and let’s start with “***settimeout()***” function.

here is the syntax :→

```javascript
setTimeout(() => {
  
}, timeout);
```

---

here is program to understand it better:→

```javascript
function hello_fn(name) {
  return `hello ${name}!!!`;
}

setTimeout(() => {
  console.log(hello_fn("ayush"));
}, 2000);
```

here “2000” is in milisecond that means == 2sec.

it’s delaying already that’s why , it’s a async task.

---

## 2&gt;Closures:→

here is the code part then we will the see the theory part :→

```javascript
function out_fn(){
  let quality = "good boy"
  return function inner_fn(name) {
    return `${name} is as ${quality}`
  }
}
let ayush_69 = out_fn();// return the inner fxn
console.log(ayush_69("ayush"));
```

---

So, here we will discuss about the theory part of the **Closure** :→

## what is “closure” ?

closure is just a function. when there is a function(outer) in that there is another function(inner) and the inner function can access outer function or variable.

## how to access the “closure” ?

so if we execute the outter\_fn. It will give me a function in return that we will save in variable(as function). we just have to execute that cz that will behave as inner\_fn().

---

# main topic :→

# callback :→

```javascript
// callback 
function doIt(a,b,cb) {
  return cb(a, b);
} 
function sub(a,b) {
  return a - b;
}
console.log(doIt(12, 13,sub));
```

this is also can be called as “higher order functions”…

## what is high order function ?

the function that take or return function as output or take as “argument” can be called as “higher order function “.

## what callback do?

callback is the function that call back the function after the task is done,,, as a function.

---

## what is set-timeout?

set-time out is also a call back function cz after 1 sec that is 1000 mili sec I was calling back the function.

```javascript
function greet(name) {
  console.log(`hello ${name}`);
}
setTimeout(greet, 1000, "Batman");
```

---

# Promise :→

as I explained in OOPs parts class and objects and discussed about it.

[click here to read about it.](https://the-os-coder.hashnode.dev/mastering-javascript-oop-a-comprehensive-guide-to-object-oriented-programming)

so what’s imp is “promise” is just a class made by node js deploper.

so is the promise section that has two part :→

a&gt; accesing the promise (mostly used and ez)

b&gt;creating a promise (hard and less will be used)

so let’s now see them one by one.

## a&gt; accessing the promise (mostly used and ez) :→

at first we don’t dive into the promise section cz that will be very overwhelming for us.

so it’s a promise given we will learn to see how to acess it.

```javascript
function fetchData() {
  return new Promise((resolve,reject) => {
    setTimeout(() => {
      let success = false;

      if (success) {
        resolve("data fetched succesfully!");
      } else {
        reject("prblm in data fetching")
      }
    }, 2000);
  })
}
//take it as black-box as of now!
```

here the code to see it :→

```javascript
///accessing the promise.
fetchData().then((data) => {
  console.log(data);
}).catch(
  (err) => {
    console.error(err);
  }
)
```

so here we can see promise are access by 2 section 1st is “,then” and other one is “.catch”

.then will get the data given by the resolve section in the promise.

1&gt; then is also higher order call back function it takes another function as “parameter”.

2&gt;in that we pass any data that will only refer to the content of the promise or the succes part.

.catch will get the data given by the reject section in the promise.

1&gt; then is also higher order call back function it takes another function as “parameter”.

2&gt;in that we pass any data that will only refer to the content of the promise or the error part.

we will under stand in the code part more better.

As we have understand it .

let’s understand the promise.

---

## b&gt;creating the promise :→

```javascript
function fetchData() {
  return new Promise((resolve,reject) => {
    setTimeout(() => {
      let success = false;

      if (success) {
        resolve("data fetched succesfully!");
      } else {
        reject("prblm in data fetching")
      }
    }, 2000);
  })
}
// making the promise
```

i&gt;promise is not made …. promise is just a class that we can access for our own async tasks.

ii&gt;promise have 2 para-meter 1st is resolve(content part) and 2nd is reject part return error part.

iii&gt;if(true) =&gt; resolve(block will run).

iv&gt;if(false) =&gt; reject(error block will run)

---

## here the full overview of the Promise :→

```javascript
function fetchData() {
  return new Promise((resolve,reject) => {
    setTimeout(() => {
      let success = true;

      if (success) {
        resolve("data fetched succesfully!");
      } else {
        reject("prblm in data fetching")
      }
    }, 2000);
  })
}
// making the promise




// consuming the promise
fetchData().then((data) => {
  console.log(data);
}).catch(
  (err) => {
    console.error(err);
  }
)
```

---

## here is the output :→

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736519037296/bc8f6053-0879-4604-bfe6-58bb2c36d566.png align="center")

---

```javascript
function fetchData() {
  return new Promise((resolve,reject) => {
    setTimeout(() => {
      let success = false;

      if (success) {
        resolve("data fetched succesfully!");
      } else {
        reject("prblm in data fetching")
      }
    }, 2000);
  })
}

fetchData().then((data) => {
  console.log(data);
}).catch(
  (err) => {
    console.error(err);
  }
)
```

---

## here is the output :→

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736519155249/001b7dfd-1430-46fb-a080-eaa276c29208.png align="center")

---

# Prototypal inheritance :→

```javascript
function Person(name,age) {
  this.name = name;
  this.age = age;
}
Person.prototype.Hello = function () {
  console.log(`${this.name} is ${this.age} old`);
}

let ayush = new Person("Batman", 18);
ayush.Hello();
```

---

## output :→

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736524579039/748e9c61-1e6a-4d5b-8c65-5a3b1ee0f4b2.png align="center")

---

# This and bind method :→

```javascript
const Student = {
  first_name: "john",
  last_name: "doe",
  age: 18,
  greetFunction() {
    return `${this.age} is very small`
  }
}
const piyush = Student.greetFunction();
const lolo = Student.greetFunction.bind({ age: 19 });
console.log(piyush);
console.log(lolo());
```

---

```javascript
// bind will make a new function.
// there is call and apply we not need to learn as of now!
// this is only valid for the context only.
```

---

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736526044415/8ceea7ec-f588-4c2a-b378-be9008df80a4.png align="center")

---

# async fxn and await :→

```javascript
async function DataAsync() {
  try {
    // all good things
  } catch (error) {
    // all error
  }
}
```

---

```javascript
function FetchDatafromApi() {
  return new Promise((resolve,reject) => {
    setTimeout(() => {
      let success = true;
     if (success) {
       resolve({ name: "Ayush", age: 19 });
     } else {
      reject("error at fetchim=ng data !!")
     }
     
   }, 1000);
    
  })
}

async function DataAsync() {
  try {
    console.log("fetching data!!!");
    const FetchedData = await FetchDatafromApi();
    console.log("the fetcged data is", FetchedData);
  } catch (error) {
   console.error("we cannot fetch the data!!!")
  }
}
DataAsync()
```

---

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736528592113/895b2431-aeec-4aa3-bdef-96322661c2ac.png align="center")

---

```javascript
function FetchDatafromApi() {
  return new Promise((resolve,reject) => {
    setTimeout(() => {
      let success = false;
     if (success) {
       resolve({ name: "Ayush", age: 19 });
     } else {
      reject("error at fetchim=ng data !!")
     }
     
   }, 1000);
    
  })
}

async function DataAsync() {
  try {
    console.log("fetching data!!!");
    const FetchedData = await FetchDatafromApi();
    console.log("the fetcged data is", FetchedData);
  } catch (error) {
   console.error("we cannot fetch the data!!!")
  }
}
DataAsync()
```

---

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736528625776/a96cdbbf-7b1e-499e-b4e9-b63e9edb4e5a.png align="center")

---

note : if there is any async fxn then only we can use await

where is promise we can use the await section.

---

and here i end the series.

---