# Javascript Interview Questions

## Table of Contents

| Sl.No | Questions                                                                      |
| ----- | ------------------------------------------------------------------------------ |
| 01.   | [What is Context in Javascript](#what-is-context-in-javascipt)               |
| 02.   | [What are Constructors in Javascript?](#what-are-constructors-in-javascript) |
| 03.   | [What is Call, Apply and Bind?](#what-is-call,-apply-and-bind)               |

<br/>

## 1Q. **_What is Context in Javascript?_**

Context is nothing but the value of `this` keyword in javascript. The `this` keyword basically refers to the object that the function is executing in.

<div align="right">
    <b><a href="#">↥ back to top</a></b>
</div>

## 2Q. **_What are Constructors in Javascript?_**

Constructors in Javascript are functions which are used to initialize a set of values or set default values for the objects.

```js
function Person(name, age, email) {
  this.name = name;
  this.age = age;
  this.email = email;
}

var myself = new Person("Abhishek", 25, "abc@gmail.com");
```

<div align="right">
    <b><a href="#">↥ back to top</a></b>
</div>

## 3Q. **_What is Call, Apply and Bind?_**

The Call, Apply and Bind methods are generally used to set the value of `this` keyword irrespective of the way in which a function is called.

<div align="right">
    <b><a href="#">↥ back to top</a></b>
</div>
