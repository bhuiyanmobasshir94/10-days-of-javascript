# 10-days-of-javascript
A basic java script fundamentals guide to the core knowledge and demonstration code snippet. There will be 10 days bootcamp here.

Day:0
=======
document.addEventListener("click",() => alert("Thanks for clicking."));

Day:1 (Values and Data types)
=======

let myName = "Mobasshir Bhuiyan Shagor"
let myNumber = 12

console.log(document.title)

document.body.style.backgroundColor = 'lightblue'

Day:2 (Function)
=======

make your own codepen at https://codepen.io

function greet(){
  alert("Hello, my name is mobasshir.");
}
greet()

function greet(name){
  alert("Hello, my name is" + name + ".");
}
greet("mobasshir")

function tripleme(x){
  return 3*x;
}

let myFavNumber = tripleMe(12)
alert(myFavNumber)

Day:3 (Objects)
================

let catName = "Fluffy"
let catAge = 4

function meow(){
  alert("Meooooowwwww!!!")
}


let cat = {
  name: "Fluffy",
  age: 4,
  foods: {
    favorite: "Tuna",
    leastFavorite: "Oranges",
  },
  eyeColor: "blue",
  meow(){
  alert("Meooowwww!!");
  }
}

// Oject contains properties and methods

cat.name 
cat.age
cat.eyeColor
cat.meow()
cat.foods.favorite
cat.foods.leastFavorite

document.addEventListener('click',myAmazingFunction)
function myAmazingFunction(){
  alert("Hello, There!");
}

Day:4 (Arrays)
==============

let myFavoriteNumber = 7
let myFavoriteNumbers = [2,3,4,5,6,7,8,9]
let myWords = ['red','orange','Yellow']
let pets = [{name:"Meowsalot",species:"cat"},{name:"Barksalot",species:"dog"}]

myWords.push() // onto the end of an existing array
console.log(myWords)

let myName = 'mobasshir'
console.log(myName.toUpperCase())

let myNumber = 7.89
console.log(myNumber.toFixed())

myWords.splice(1,1) // index,how many number

console.log(myFavoriteNumbers[1])

console.log(myPets[1].species)

Day:5 (Decisions)
==================

let strawberryCount = 20
if (strawberryCount > 9 ){ // any larger than 0 is true // it is really expected for true and false
  document.write("Congrats!")
}else{
  document.write("Sorry, we do not ship orders that small.")
}

let testValue = true
let testValue = false 

while(true){
  document.write("Some writings");
}

let count = 2
while (count <= 200){
  document.write(count);
  count += 1;
}


Day:6 (Higher Order Functions)
===============================

1) Accepts a function as an argument.
2) Returns a function.

document.addEventListener('click', ourAmazingFunction);

function ourAmazingFunction(){
  alert("Thank you for clicking.");
}

function doubleMe(x){
  return x*2;
}

function tripleMe(x){
  return x*3;
}

function quadrupleMe(x){
  return x*4;
}

document.write(doubleMe(20))

function createMultiplier(multiplier){
  return function(x){
    return x * multiplier
  }
}

let doubleMe = createMultiplier(2)
let tripleMe = createMultiplier(3)
let quadrupleMe = createMultiplier(4)

document.write(doubleMe(12))
document.write(tripleMe(12))
document.write(quadrupleMe(12))

let myColors = ['red','orange','yellow']
myColors.forEach(saySomethingnice)

function saySomethingNice(color){
  document.write(color)
}

myColors.map()
myColors.filter()


Day:7 (returning and mutating)
=============================

let pets = [
{name; "Meowalot", species: "cat", age: 2},
{name: "Barksalot", species: "dog", age: 7}
]

pets.push()

pets.map(nameOnly)

function nameOnly(pet){
  return pet.name
}

let dogs = pets.filter(onlyDogs)

function onlyDogs(pet){
  return pet.species == "dog"
}

function onlybabies(pet){
  return pet.age < 3
}

let babyDogNames = pets.filter(onlyDogs).filter(onlyBabies).map(nameOnly)

Day:8 (Scope and Context)
============================

// scope is a biggest source of confusion regarding variables.
// context is the biggest source of confusion regarding objects.

let myName = 'mobasshir'

function amazingFunction(){
  let myName = 'Brad Junior';
  if(2+2 == 4){
    let myName = 'Bhuiyan';
    console.log(myName);
  }
}

amazingFunction()

// let uses block scope
// var uses fuction scope


let john = {
  firstName: "john",
  lastname: "Doe",
  driveCar(){
    function iAmFunction(){
      console.log(this)
    }
    iAmFunction()
    console.log(this.fistName + " " + this.lastName + "is driving a car.");
  }
}

john.driveCar()

function breathe(){
  console.log(this.fistName + " " + this.lastName + " just inhaled and exhaled.");
}

breathe.call(john)
// window is a top level global object

// The thid kkeyword points towards the object that is executing the current function

Day:9 (Miscellaneous)
=======================

document.addEventListener("clicl",()=>alert("Thank you for clicking!"))

let myNumbers = [20,400,650]
let doubledNUmbers = myNumbers.map(x => x*2)
console.log(doubledNumbers)

// function hoisting

cool()
function cool(){
  console.log("hey...")
}

let myName = 'mobasshir'
console.log(`Hello, my name is ${myName}. I am a bad guy.`)

Day:10 (Web browser Practices)
===============================

    <h1> To-Do-App </h1>

    <form id="ourForm">
      <input id="ourField" type="text" autocomplete="off">
      <button> Create item </button>
    </form>

    <h3> Need to do</h3>
    <ul id="ourList">

    </ul>

    <script>
      let ourForm = document.getElementById("ourForm")
      let ourField = document.getElementById("ourField")
      let ourList = document.getElementById("ourList")

      ourForm.addEventListener("submit",(e)=>{
        e.preventDefault()
        createItem(ourField.value)
      })

      function createItem(x){
        let ourHTML = `<li>${x} <button onclick="deleteItem(this)">Delete</button></li>`
        ourList.insertAdjacentHTML('beforeend',ourHTML)
        ourField.value = ""
        ourField.focus()
      }

      function deleteItem(item){
        item.parentElement.remove()
      }
    </script>


