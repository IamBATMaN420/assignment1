---
title: "HTML Basics to Advanced: The Complete Guide for Beginners"
seoTitle: "Understanding HTML: The Building Blocks of the Web"
seoDescription: "Discover the essentials of HTML, the backbone of every website. Learn its structure, importance, and tips to create stunning, responsive web pages with this"
datePublished: Sat Nov 23 2024 13:23:48 GMT+0000 (Coordinated Universal Time)
cuid: cm3u7bby5000d09l7el6gegfp
slug: html-basics-to-advanced-the-complete-guide-for-beginners
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1732427389941/5b443407-d8b8-400c-8921-1658f4212192.jpeg
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1732427442852/1831fc69-71b3-4a92-9fac-c0afdd0e4a93.jpeg
tags: web-development, webdev, full-stack, html5, frontend-development

---

---

**Description:**  
Learn HTML, the foundation of web development, with this comprehensive guide. Explore everything from basic tags and structure to advanced techniques like forms, multimedia integration, and semantic elements. Perfect for beginners looking to build professional, user-friendly websites.

---

# a&gt; Basics of html and basic tags :→

html :-&gt; hyper text markup language

meta data :-&gt; info about the anything. ([mp3.mp](http://mp3.mp)4)

1&gt; doctype html (is saying) hey my document type is html )

2&gt; html don’t know about space

3&gt; 6 heading (h1---h6)

```xml
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>basic-html-by-ayush</title>
</head>
<body>
  <h1>hello world!</h1>
  <h2>hello world!</h2>
  <h6>hello world!</h6>
</body>
</html>
```

4&gt;Emmet is give short cur for ez part and also give in vs code by default

5&gt;ul&gt;li\*3 =&gt; 3 li in ul (emmet)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1729859017415/f9efc571-f349-43c6-86ef-b7af4029fa3a.png align="center")

```xml
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>lists</title>
</head>
<body>
  <ul> <!--un-ordered list-->
    <li>apple</li>
    <li>mango</li>
    <li>banana</li>
  </ul>
  <ol>
    <li>apple</li>
    <li>mango</li>
    <li>banana</li>
  </ol>
  
</body>
</html>
```

6&gt;block line element =&gt; take the whole line space and block the space

7&gt;inline elements =&gt; take the only space given

8&gt;list =&gt; ol and ul more over there list items will be shown in "li" format

9&gt; ol =&gt; ordered list ul =&gt; un-ordered list and li=&gt; list items

10&gt;block level items :-&gt;

a&gt;heading h1 to h6(that will give headings)

b&gt;ol, li

c&gt;li

d&gt;p

e&gt;div

11&gt; inline elements =&gt;

a&gt;span

b&gt;iimg

c&gt;a tag

12&gt; tag is a img,a

14&gt; attribute is href and width height

```xml
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>image</title>
</head>
<body>
 
<img src="source" alt="about the pic">
<!-- image is self closing tag -->
<a href="souce link"></a>
  
</body>
</html>
```

15&gt; controls can control video audio and all

16&gt; we can go to mdn documentation and learn all

17&gt; there is semantic tag =&gt; that means tag which have meaning like =&gt; a&gt;nav

b&gt;header

c&gt;footer and everything which have any meaning

18&gt;tr =&gt; table row and td =&gt; table data

19&gt;in tr there will be td

20&gt;all will be in table tag

```xml
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>table</title>
  </head>
  <body>
    <table class="login">
      <tr>
        <td>name</td>
        <td>email</td>
        <td>pasword</td>
      </tr>
    </table>
    <table>
      <tr>
        <td>ayush</td>
        <td>basakayush942@gmail.com</td>
        <td>test1</td>
      </tr>
    </table>
    <!--make basic table-->
  </body>
</html>
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1729859409030/c2689e2c-ed75-48bd-9b24-c55978799ad6.png align="center")

21&gt;action in the form show where the data of the form to be gone

## b&gt;Forms in HTML

```xml
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>FORM</title>
  </head>
  <body>
    <label for="basics">
      <form action="place where the data go">
        E-mail:<input type="email" name="email" id="" /> basketball:<input
          type="checkbox"
          name="basketball"
          id=""
        />
        football:<input type="checkbox" name="" id="" /> hindu:<input
          type="radio"
          name=""
          id=""
        />
      </form>
    </label>
  </body>
</html>
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1729862048925/211934e7-e7a7-43a0-a23c-974bc083448c.png align="center")

22&gt;by title =&gt; tooltip is given

```xml
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>tooltip</title>
  </head>
  <body>
    <img src="./webp.webp" alt="" width="200px" title="html logo">
  </body>
</html>
```

![]( align="center")

\=&gt; here is no code the code part will be done by exercises only

---

\-by Ayush Basak(full stack dev)

---

# c&gt;11 task of html

1&gt;Coding Exercise 1: Create a Simple Heading

2&gt;Coding Exercise 2: Create a Paragraph with a Link

3&gt;Coding Exercise 3:tooltip on hover

4&gt;Coding Exercise 4:make a button

5&gt;Coding Exercise 5:make an unordered list

6&gt;Coding Exercise 6:make simple table

7&gt;Coding Exercise 7:make a form with input field

8&gt;Coding Exercise 8:make a form with dropdown menu

9&gt;Coding Exercise 9:make a image with alt text

10&gt;Coding Exercise 10:hyperlink that will open on new tab

11&gt;Coding Exercise 11:create progress bar in html

---

# d&gt;11 task solution to master “HTML” :→

## In the previous page you will get 11 task to master html

---

### 1&gt;Coding Exercise 1: Create a Simple Heading

```xml
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>task1</title>
</head>
<body>
  <!--CREATING A SIMPLE HEADING-->
  <h1>HELLO WORLD</h1>
</body>
</html>
```

### 1&gt;OUTPUT OF TASK-1 IS:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1729863224327/3f2d989d-4934-4dcd-bb7e-d438cffa8bac.png align="center")

---

### 2&gt;Coding Exercise 2: Create a Paragraph with a Link

```xml
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>task2</title>
</head>
<body>
  Lorem <a href="https://www.linkedin.com/in/ayush-basak1/">ipsum dolor</a>, sit amet consectetur adipisicing elit. Labore culpa atque cum perferendis! A quis exercitationem laboriosam est velit explicabo! Debitis nisi nam quasi minus neque reiciendis facilis voluptatibus ipsum!
  Cupiditate corrupti, eius eaque atque ullam ratione dolorem laboriosam veritatis optio, praesentium rem consectetur sequi, consequatur facilis velit ut mollitia cumque sapiente delectus in! Dolorum earum laborum perspiciatis aliquam quisquam!
</body>
</html>
```

### 2&gt;output:→

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1729863514715/9ff46227-ced4-4250-8399-c3483f768e21.png align="center")

---

### 3&gt;Coding Exercise 3:tooltip on hover

```xml
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>task3</title>
</head>
<body>
  <!--Coding Exercise 3:tooltip on hover-->
  <img src="./index.html" alt="html" width="60%" title="html logo">
</body>
</html>
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1729864067815/fe5e2e7b-b524-4686-aea1-c2a79c5e41d9.png align="center")

---

### 4&gt;Coding Exercise 4:make a button

```xml
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>task3</title>
  </head>
  <body>
    <!--4>Coding Exercise 4:make a button-->
    <label for="login">
      <button>login</button>
    </label>
  </body>
</html>
```

### 4&gt;output:→

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1729864286181/734d8c40-b82a-4bbc-8bde-0369241b9dfc.png align="center")

---

### 5&gt;Coding Exercise 5:make an unordered list

```xml
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>task5</title>
  </head>
  <body>
    <!--Coding Exercise 5:make an unordered list-->
    <ul>
    urordered list :->
      <li>appple</li>
      <li>banana</li>
      <li>pitch</li>
    </ul>
  </body>
</html>
```

### 5&gt;output:→

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1729864482280/a0003feb-b30e-42cc-8f70-bce5b9965b0e.png align="center")

---

### 6&gt;Coding Exercise 6:make simple table

```xml
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>task6</title>
  </head>
  <body>
    <!--6>Coding Exercise 6:make simple tablew-->
    <table>
      <td>
        <tr>
          name
        </tr>
        <tr>
          dept
        </tr>
        <tr>
          roll
        </tr>
      </td>
      <table>
        <td>
          <tr>
            ayush
          </tr>
          <tr>
            eco
          </tr>
          <tr>
            1
          </tr>
        </td>
      </table>
      <table>
        <td>
          <tr>
            piyush
          </tr>
          <tr>
            maths
          </tr>
          <tr>
            2
          </tr>
        </td>
      </table>
    </table>
  </body>
</html>
```

### 6&gt;output:→

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1729864937178/4872e13e-d927-4bfb-adba-cbd6a0dfd1ad.png align="center")

---

### 7&gt;Coding Exercise 7:make a form with input field

```xml
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>task7</title>
</head>
<body>
  <!--make a form with input field-->
  <label for="login">
  <form action="to where the dat will go">
    name: <input type="text" placeholder="name">
    E-mail: <input type="email" name="email" id="">
    phone-number: <input type="number" name="number" id="">
    <button>login here</button>
  
  </form>
</label>
</body>
</html>
```

### 7&gt;output:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1729865243733/f5e82256-f030-4a51-89b8-b59563fa5a01.png align="center")

---

### 8&gt;Coding Exercise 8:make a form with dropdown menu

```xml
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>task8</title>
  </head>
  <body>
    <!--8>Coding Exercise 8:make a form with dropdown menu-->

    <form action="go where the dats is important ">
      <select name="games" id="">
        <option value="pubg">pubg</option>
        <option value="bgmi">bgmi</option>
        <option value="valorant ">valorant</option>
      </select>
    </form>
  </body>
</html>
```

### 8&gt;output:→

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1729865761247/fc2e15ee-c2ee-4855-be70-fb4f5dd16d9d.png align="center")

---

### 9&gt;Coding Exercise 9:make a image with alt text

```xml
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>task9</title>
  </head>
  <body>
    <!--9>Coding Exercise 9:make a image with alt text-->
    <img src="/webp.webp1" alt="htmllogo" width="200px">
  </body>
</html>
```

### 9&gt;output

here we give the wrong link if the picture and alt attribute used when the pic will break it will give alt text to us

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1729865981684/e7feeda7-508e-477b-ac37-17a3ea05b311.png align="center")

---

### 10&gt;Coding Exercise 10:

### hyperlink that will open on new tab

```xml
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>tast-10</title>
</head>
<body>
  <a href="https://www.linkedin.com/in/ayush-basak1/" target="_blank"></a>
</body>
</html>
```

### 10&gt;output→

so the anchor tag (a) there is a attribute named =&gt;”target=\_blank” this will open an other tab .

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1729866452991/3a7d0bba-f37e-40b6-a632-71e2fb024d51.png align="center")

---

### 11&gt;Coding Exercise 11:create progress bar in html

```xml
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>tast-11</title>
  </head>
  <body>
    <!--11>Coding Exercise 11:create progress bar in html-->
    <label for="progress in file upload"> file uploading:-> </label>
      <progress id="file" value="50" max="100">
        50
      </progress>
    
  </body>
</html>
```

### 11&gt;output:→

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1729866948750/ad9abc9c-6000-4430-8686-aecd4fab41c1.png align="center")

---

**HTML Basics Summary**

This guide covers the foundational concepts of HTML, the backbone of web development. Whether you're just starting or brushing up your skills, this summary walks you through the essentials:

* **Introduction to HTML**: Understanding the role of HTML as a markup language to structure web content, with examples of basic tags like `<html>`, `<head>`, and `<body>`.
    
* **HTML Structure**: Explanation of metadata, the purpose of `<!DOCTYPE html>`, and the nature of block-level and inline elements.
    
* **Lists**: Creating ordered (`<ol>`) and unordered (`<ul>`) lists, along with Emmet shortcuts for efficient coding.
    
* **Images and Links**: Incorporating images with `<img>` and hyperlinks with `<a>`, using attributes like `src`, `alt`, and `target`.
    
* **Tables and Forms**: Designing basic tables with `<table>`, `<tr>`, and `<td>`, and creating forms with input fields, checkboxes, radio buttons, dropdowns, and action attributes.
    
* **Semantic Elements**: Using meaningful tags like `<nav>`, `<header>`, and `<footer>` to improve readability and accessibility.
    
* **Interactive Elements**: Exploring tooltips, progress bars, and media controls.
    
* **Hands-On Tasks**: Eleven practical exercises ranging from creating headings and lists to building forms and progress bars, solidifying your grasp of HTML concepts.
    

**Conclusion**

With this guide, you've gained a solid understanding of HTML basics, from tags and structure to advanced elements like forms and tables. By completing the hands-on tasks, you’ve built a strong foundation for web development. The next step is diving into CSS to bring your web pages to life with styling and design.

Onward to CSS—where creativity meets structure!

---

## — by Ayushthebatman (Full stack dev)

---