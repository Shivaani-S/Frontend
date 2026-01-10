# 1. we define function like this 

function main()
{

}
instead we use arrow function..

const add = (a,b) =>{
    return a+b;
};


# 2.Use of ternary operator instead of if else

let name= age>10 ? "alice" : "bob"


# 3.objects --> ES6 FEAUTURES MADE OBJECT HANDLING WAY MORE EASIER!
# 1.property shorthand
let person={
    name: "Shivaani",
    age: 18

};
this is an object and

name="shivaani"
age=18

let girl={
    name:name,
    age:age
};

we can use 
let girl = { name, age };


# 2.method shorthand
  

  old way:
  let user = {
  greet: function () {
    console.log("Hi");
  }
};


ES6 way:

let user = {
  greet() {
    console.log("Hi");
  }
};

# 3.destructuring 

let user = { name: "Shivv", age: 19 };

instead of :

let name = user.name;
let age = user.age;

use this :
let { name, age } = user;

console.log(name); // "Shivv"
console.log(age);  // 19

# 4.Spread Operator (...)

Copy or merge objects.

let a = { x: 1 };
let b = { y: 2 };

let c = { ...a, ...b };
Result:
{ x: 1, y: 2 }


also in arrays we can use like
a=["apple","banana","orange"]
b=[...a , "mango"]

# 5.Computed Property Names:

Use a variable’s value as the object key.

let key = "score";
let obj = { [key]: 100 }; // { score: 100 }


No brackets → key is the literal word.

Brackets [ ] → key comes from the variable.


### 3 fundamental functions !
.map()
.filter()
.reduce() --> not used mainly

 