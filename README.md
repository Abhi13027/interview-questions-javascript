# Javascript Interview Questions

## Table of Contents

| Sl.No | Questions                                                                    |
| ----- | ---------------------------------------------------------------------------- |
| 01.   | [What is Context in Javascript?](#what-is-context-in-javascript)             |
| 02.   | [What are Constructors in Javascript?](#what-are-constructors-in-javascript) |
| 03.   | [What is Call Apply and Bind?](#what-is-call-apply-and-bind)                 |
| 04.   | [What is SetTimeout?](#what-is-settimeout)                                   |

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

`Call()`<br/>
The call method executes the function with a given <i>this</i> value with arguments provided individually.

```js
var obj1 = {
  num: 3,
};

var addTo = function (a, b, c) {
  return this.num + a + b + c;
};

console.log(addTo.call(obj1, a, b, c));
```

`Apply()`<br/>
The apply method is exactly the same as the call method in functionality. The only difference is that the arguments are provided in an array.

```js
var obj2 = {
  num: 3,
};
var addTo = function (a, b, c) {
  return this.num + a + b + c;
};

var arr = [8, 8, 9];

console.log(addTo.apply(obj2, arr));
```

`Bind()`<br/>
The bind method creates a new function that when called has it's <i>this</i> keyword set to the provided value.

```js
var obj3 = {
  num: 3,
};

var addTo = function (a, b, c) {
  return this.num + a + b + c;
};

var newFunc = addTo.bind(obj3);

console.log(newFunc(8, 8, 9));
```

<div align="right">
    <b><a href="#">↥ back to top</a></b>
</div>

4. ### What is SetTimeout?

The SetTimeout function calls the function or evaluates the function after a specified number of milliseconds.

```js
setTimeout(function () {
  console.log("Hello World!");
}, 2000);
```

`Hello World!` will get printed after 2 seconds (2000 milliseconds).

<div align="right">
    <b><a href="#">↥ back to top</a></b>
</div>
