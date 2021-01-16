# Javascript Interview Questions

## Table of Contents

| Sl.No | Questions                                                                    |
| ----- | ---------------------------------------------------------------------------- |
| 01.   | [What is Context in Javascript?](#what-is-context-in-javascript)             |
| 02.   | [What are Constructors in Javascript?](#what-are-constructors-in-javascript) |
| 03.   | [What is Call Apply and Bind?](#what-is-call-apply-and-bind)                 |

<br/>

1. ### What is Context in Javascript?

Context is nothing but the value of `this` keyword in javascript. The `this` keyword basically refers to the object that the function is executing in.

```js
var person = {
  name: "Aman",
  age: 25,
  hello: function(){
    console.log(this);
  }
}

person.hello();

{name: "Abhishek", age: 25, hello: [Function: hello]}
```

<div align="right">
    <b><a href="#">↥ back to top</a></b>
</div>

2. ### What are Constructors in Javascript?

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

3. ### What is Call, Apply and Bind?

The Call, Apply and Bind methods are generally used to set the value of `this` keyword irrespective of the way in which a function is called.

<div align="right">
    <b><a href="#">↥ back to top</a></b>
</div>
