---
title: "Mastering BOM and DOM in JavaScript: 9 Practical Exercises"
seoTitle: "Mastering BOM and DOM in JavaScript: 9 Practical Exercises"
seoDescription: "Confused about BOM and DOM in JavaScript? This blog explains both concepts in detail with 9 fun and educational exercises"
datePublished: Tue Dec 10 2024 01:38:36 GMT+0000 (Coordinated Universal Time)
cuid: cm4hslwtj000208jlhybl4197
slug: mastering-bom-and-dom-in-javascript-10-practical-exercises
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1733794593835/0454de14-960d-44de-8ba5-215e3b0b7b6f.webp
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1733794660303/44d7620b-6c60-4594-80b5-4e9c94d4d473.webp
tags: js, javascript, dom, functional-programming, frontend-development, dom-manipulation

---

Description:→ Confused about BOM and DOM in JavaScript? This blog explains both concepts in detail with 9 fun and educational exercises.

---

# 1&gt;BOM(browser object model):→

So, by manipulating “BOM” we can see the changes in the browser. And js helps us to interact with “browser” element.

It’s distinct from “DOM” .

---

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1733797580679/cb7a3b38-46fd-472e-9171-17b94c71f0a9.png align="center")

---

## here is a pictorial representation where we have show some “BOM” properties.

here is it :→

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1733798285935/a54fb03d-e998-4474-9984-e840f338ccff.png align="center")

---

### now let’s code and verify that. :”)

so here we have made html document where we have to make → “udex.html” , then we have to make “js” file name →”script.js”. And we have to open it on “<mark>Live server</mark>”. Then use some “<mark>BOM</mark>” … with ”<mark>window</mark>” object. In “<mark>BOM</mark>” there is 3 objects they are (by which we can let go the “BOM” and have to go to “DOM”) :→

## a&gt;navigator

## b&gt;location

## c&gt;screen

```xml
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>BOM</title>
</head>
<style>
  body{
    background-color: #1a1a1a;
    color: aliceblue;
  }
</style>
<script src="./script.js"></script>
<body>
  <h1>Lorem ipsum dolor sit amet consectetur.</h1>
</body>
</html>
```

---

here is the “Javascript” code we want to connect with “HTML”

```javascript
console.log("hello world!!")
console.log(location.href);// location
console.log(navigator.userAgent)//navigator
console.log(screen.width)// screen width
console.log(screen.height)// screen height
console.log(window.location)// window object
```

---

## here is the output from “BOM“ is :→

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1733804653760/a72a2e22-2eaa-401a-845f-dd09afc23082.png align="center")

---

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1733804687106/18c70056-a571-416b-b92e-ebd22c692121.png align="center")

---

# 2&gt;DOM(document object model) :→

after BOM there is “DOM”.

There only 2 part of DOM we need to master :→

### 1&gt; getting elements

### 2&gt; add the event listener

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1733836079473/cbd898ce-6365-41bd-ada2-223b1aac31b9.png align="center")

---

that’s all theory we need in this section here we will learn every thing from hands on experience with 9th problem :→

```xml
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>DOM</title>
    <style>
      body {
        background-color: #1a1a1a;
        color: aliceblue;
        /* justify-content: center;
        align-items: center;
        height: 100vh; */
      }
      .highlight {
        background-color: yellow;
        color: #1a1a1a;
      }
      .text-align-container {
        text-align: center;
      }

      #center-button {
        padding: 10px 20px;
      }
    </style>
  </head>
  <body>
    <!-- 1st problem:→click on the button change the text :→ -->
    <h1>1st problem</h1>
    <h1 id="para-1">Lorem ipsum dolor sit amet consectetur.</h1>
    <button id="change-text">LogIn</button>
    <hr />

    <!--2nd prblm:-> traversition of DOM i.e. when we click on button the fist thing will be highlighted -->
    <h1>2nd problem</h1>
    <h1 id="para-2">traversition of DOM</h1>
    <ol id="list">
      <li class="first-list">mango</li>
      <li>apple</li>
      <li>lichi</li>
      <li>bannana</li>
    </ol>
    <button id="change-button">click me!</button>
    <hr />

    <!--3rd problem:-> manipulating the DOM element :-> make biriyani to momo-->
    <h1>3rd problem</h1>
    <h3 id="finalorder">
      <div id="food">order: <span id="biriyani">biriyani</span></div>
    </h3>
    <button id="change">change me !!!</button>
    <hr />
    <!--4th problem :-> here we will learn about creating  and inserting the DOM elements-->
    <h1>4th elements</h1>
    <ul id="tasklist">
      <li>momo</li>
      <li>fried-rice</li>
      <li>biriyani</li>
    </ul>
    <div class="text-align-container">
      <button id="center-button">Click Me!</button>
    </div>

    <hr />

    <!--5th problem:-> deleting some item in "DOM"-->
    <h1>5th problem</h1>
    <h2>
      <ul id="del-list">
        <li>mango</li>
        <li>lichi</li>
        <li>guava</li>
        <li>watermelon</li>
      </ul>
      <button id="delete">delete item</button>
    </h2>

    <hr />

    <!--6th problem:-> Event Delegation in "DOM"-->
    <h2>6th problem</h2>
    <ul id="myList">
      <!--in this delegation there is one parent class 
      and the job is instead of writimg every event-listener
      we will just write for one. And child will just follow it.
      -->
      <li style="cursor: pointer">Item 1</li>
      <li style="cursor: pointer">Item 2</li>
      <li style="cursor: pointer">Item 3</li>
    </ul>
    <hr />
    <!--7th problem:-> FORM handling in "DOM"-->
    <h2>7th problem</h2>
    <style>
      #feedback_form {
        font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
      }
    </style>
    <form
      action=""
      id="feedback_form"
      style="display: flex; align-items: center; justify-content: center"
    >
      <label for="feedback_form" style="margin: 10px"
        >Your feedback is:-></label
      >
      <input type="text" id="input_feild" required />
      <button type="submit" class="btn btn-primary" id="submit_btn">
        Submit
      </button>
    </form>
    <div
      id="feedback_rep"
      style="
        background-color: blueviolet;
        border: 3px solid #1a1a1a;
        padding: 10px;
        margin: 10px;
      "
    ></div>
    <hr />
    <!-- 8th problem: dom content is loaded -->
    <section id="example-8">
      <h2>DOM is loaded!!!</h2>
      <p id="domstatus">waitting for the DOM to load...</p>
    </section>
    <hr />

    <!-- 9th problem: toggle the highlight -->
    <h1><div>9th problem</div></h1>
    <p id="toHighlight">toggle the text !!!</p>
    <button id="toHighlight_btn">toogle this</button>
    <script src="./script.js"></script>
  </body>
</html>
```

---

```javascript
// example-1
document.getElementById("change-text").addEventListener("click", function () {
  document.getElementById("para-1").textContent = "You have done it!!!";
});

// example-2
document.getElementById("change-button").addEventListener("click", function () {
  document.getElementById("list").firstElementChild.classList.add("highlight");
});
// classlist is used when we have to add remove or perform anything. that's why we have to use that.

// example-3
document.getElementById("change").addEventListener("click", function () {
  document.getElementById("biriyani").textContent = "MOMO";
});

//example-4 :->
document.getElementById("center-button").addEventListener("click", function () {
  let newItem = document.createElement("li");
  // to make it
  newItem.textContent = "soups!";
  // add the text content
  document.getElementById("tasklist").appendChild(newItem);
  // select the tastlist and appendchild means make a child in li group and add new item
});

//example-5->
document.getElementById("delete").addEventListener("click", function () {
  let delete_button = document.getElementById("del-list");
  delete_button.lastElementChild.remove();
});

//example-6 :->
const list = document.getElementById("myList");

list.addEventListener("click", function (event) {
  // Check if the clicked element is a list item
  if (event.target && event.target.nodeName === "LI") {
    alert("You clicked on" + " " + event.target.textContent);
  }
});

//example:-> 7
document
  .getElementById("feedback_form")
  .addEventListener("submit", function (event) {
    event.preventDefault();
    let feedback = document.getElementById("input_feild").value;
    document.getElementById(
      "feedback_rep"
    ).textContent = `your feedback is ${feedback}  `;
  });

//example-8
document.addEventListener("DOMContentLoaded", function () {
  document.getElementById("domstatus").textContent = "your DOM is loaded!!!";
});

//example-9
document
  .getElementById("toHighlight_btn")
  .addEventListener("click", function () {
    let toggle_69 = document.getElementById("toHighlight");
    toggle_69.classList.toggle("highlight")
  });
```

---

<details data-node-type="hn-details-summary"><summary>Blog Post: Understanding the DOM in JavaScript</summary><div data-type="detailsContent"></div></details>

#### **Domain Summary**

The Document Object Model (DOM) is a programming interface for web documents. It represents the structure of a webpage as a tree-like hierarchy, enabling developers to manipulate HTML and CSS dynamically using JavaScript. Key points include:

1. **What is the DOM?**
    
    * A structured representation of a webpage.
        
    * Allows interaction with elements (like text, images, and buttons).
        
2. **Core Features of the DOM**:
    
    * **DOM Elements**: Nodes representing HTML tags (e.g., `<div>`, `<p>`).
        
    * **DOM Manipulation**: Add, remove, or change elements dynamically.
        
    * **Event Handling**: Respond to user actions like clicks or keypresses.
        
3. **Common JavaScript Methods for DOM Interaction**:
    
    * `getElementById()`, `querySelector()`: Access elements.
        
    * `createElement()`, `appendChild()`: Add new elements.
        
    * `addEventListener()`: Handle events like clicks or form submissions.
        
4. **Why It Matters**:
    
    * Enables dynamic and interactive web experiences.
        
    * Forms the foundation of modern web development practices like React or Angular.
        

#### **Conclusion**

In conclusion, the DOM is at the heart of JavaScript's ability to make webpages dynamic and user-friendly. Understanding how to traverse, manipulate, and listen to events within the DOM empowers developers to create engaging web applications. Whether you're adding a new button, updating content on the fly, or building complex front-end frameworks, mastery of the DOM is essential.

Ready to get started? Explore these concepts by building a simple webpage and experimenting with DOM methods. What will you create today? Now from here on-wards we will go through to “<mark>Advance (async) JavaScript</mark>”.

## \-AyushtheBatman(full stack devloper)

---