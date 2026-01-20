# What is JAVASCRPT?
  -JavaScript is a high-level, interpreted, dynamically typed programming language used to create interactive and dynamic web pages. It runs in the browser and can also run on servers using environments like Node.js.

# VARIABLES:
 - A variable is a named storage in memory that holds data which can be changed during program execution. It acts as a container for values like numbers, strings, or objects.

   var a=10  ---> variable declaration!
   var b=20
   console.log(a+b) --> prints 30

   # three are three types of declaring a variable
     -  var
     -  let
     -  const
     
#  var (global scope)

- Scope: Function-scoped. Accessible anywhere inside the function where declared.
- Re-declaration: Can re-declare in the same scope.
- Update: Can be updated.
- Hoisting: Hoisted and initialized as undefined
        
# let
 
 - scope: block scoped ({ accessible only inside this block})
 - cannot be re-declared but can be updated 
 - hoisted but in temporal dead zone(tdz means the period between the start of the block and the moment let or const variable is declared (not for var only let and const)during which the variable exists but cannot be accessed.)

# const
  - block scoped
  - cannot be updated or redeclared
  - hoisted but in tdz


- strings should be given inside "(string)"
- if u declare var a =apple it will think inside a variable "a" there is aother varaible called "apple" and check inside it for value.

# keywords:
- predefined words which cant be used as varaible !
e.g let, const, if ,switch etc

#commments 

// -->single line comment
/* */ multiline comment


# Datatypes

- JS is dynamically typed language which declares the type of a variable during runtime.
- ![JS DATATYPES](image.png)


# js function

code: 
 function greet()
{
    console.log("hi!")
}
greet();


### JAVASCRIPT DOM(DOCUMENT OBJECT MODEL)MANIPULATION

- DOM manipulation means using JavaScript to change what you see on a webpage without reloading the page.
- DOM means the HTML code of a webpage is represented as a tree structure in the browser’s memory.


# Event:
- An event is any action performed by the user or browser, like a click, key press, or page load. eg : clciking a button ,hovering mouse.

# EVENT HANDLER
- An event handler is a function that runs when an event occurs


e.g code
<input type="text" id="num1">
<input type="text" id="num2">
<button onclick="add()">ADD</button>
<p>
    Result:
</p>
<script>
function add()
{
    let num=+document.getElementById("num1").value  //here + refers to number u can also use Number()
    let numm=+document.getElementById("num2").value
    console.log(num+numm)

}
</script>


# Math Random
let b=Math.random()
---> this generates a number between 0 to 1
we  multiply it by 10 to give a num between 0 and 9 in double
and we use Math.floor to only get the first value.

e.g code 


let b=Math.random()*10
console.log(b)
let c=Math.floor(b)
console.log(c)


# Now lets do a guess a number game!





<h1>Guess the number!</h1>
<input id="input">
<button onclick="check()">check</button>
<p id="result">result:</p>

<script>
 function check()
 {
    let num=Math.floor(Math.random()*10)
    let guess=+document.getElementById("input").value 
    if (num==guess) 
 {
    document.getElementById("result").textContent="You found it!"
 }

 else
 {
    document.getElementById("result").textContent="wrong answer!"
 }
 }



</script>



# Now let's see how to manipulate css using js

## example code

<div id="res"></div>
<button onclick="changecolor()">Change Color</button>
<style>
    div{
        width: 300px;
        height: 300px;
        background-color: black;
        transition: 2s;
    }
    .height
    {
        height: 900px;
    }
</style>

<script>
    function changecolor()
    {
        let box=document.getElementById("res")
        box.style.backgroundColor="yellow"
        box.setAttribute("class","height")

 
    }
</script>




GO THROUGH ON HOW TO USE ![alt text](image-3.png)






## Task 1: WHENVER YOU TYPE SMTHG ON INPUT BOX IT SHOULD APPEAR BELOW ONSPOT WITHOUT REFRESHING AUTOMATICALLY

<input id="input" onkeyup="clickk()">
<h1 id="result">Result</h1>

<script>
    function clickk()
    {
       
       let c=document.getElementById("input").value
       document.getElementById("result").textContent=c
    }
</script>


# onkeyup is used

## Task 2 :

![alt text](image-1.png)

<button onclick="update()">Add</button>
<div id="res"></div>
<script>
 let item=document.getElementById("res")
 
function update(){
    let list=document.createElement("h1")
    list.textContent="hello"
    item.append(list)
 }
</script>


## TASK 3: button on click should change it's(button) color

<button onclick="change()" id="btn">Change color</button>
<script>
  function change()
  {
   let button=document.getElementById("btn")
   button.style.backgroundColor="red"
  }
</script>

## TASK 4:
![alt text](image-2.png)

<h1 id="name">name</h1>
<button onclick="namechange(event)">John</button>
<button onclick="namechange(event)">Hari</button>
<button onclick="namechange(event)">Praveen</button>

<script>
    let h1=document.getElementById("name")
    function namechange(event)
    {
        h1.textContent=event.target.textContent
    }
</script>




## Learn the use of innerhtml and how to use it to manipulate the code

## TASK 5:
 <h1 id="res">Hello</h1>
<button onclick="change()">Click</button>
<script>
  let text=document.getElementById("res")
  function change()
  {
    if(text.textContent=="Hello")
      text.innerHTML="Bye"

      else if(text.textContent=="Bye")
      text.innerHTML="Hello"
  }
</script>


## Task 6:

<input id="input" oninput="wordcount()">
<h1 id="count">Count:</h1>
<p id="warn"></p>

<script>
     let input=document.getElementById("input")
    
     let count=document.getElementById("count")
     
     let warn=document.getElementById("warn")
     let max=10
     function wordcount()
     {
        let len=input.value.length
        if(max<= len)

        {
            warn.textContent="words exceeds the maximum limit!"
            warn.style.color="Red"
        }
         else
         {
          count.textContent="Count: "+len
          warn.textContent=""
         }
     }
</script>


## Task 7:

<h1>heelloo guys !!!</h1>
<h2>This is my new website!!!</h2>
<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat voluptates magni vero doloribus, temporibus incidunt dolorum, a dignissimos autem ratione, repudiandae sit error totam! Repellendus sunt magni reprehenderit ipsam sint!</p>
<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sint vero praesentium aliquid. Dolore dolores possimus ipsam omnis magni optio praesentium tempora molestiae repudiandae consequuntur eum inventore nam vero iusto harum, accusantium soluta? Illum minima saepe nam maxime quas nostrum accusantium, culpa, rem, porro natus repudiandae nobis ratione. Quisquam, perferendis culpa?</p>
<button onclick="toggle()">togglelight</button>
<style>
    body{
        background-color: black;
        color: white;
        transition: background-color 2s ease;
    }
    .dark{
        background-color: white;
        color: black;
    }
</style>
<script>
    
     function toggle()
     {
          document.body.classList.toggle("dark")
     }
</script>






## check the projects in project folder too!!!! 