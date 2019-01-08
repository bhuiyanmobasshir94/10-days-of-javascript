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


Day:7 (returning and muting)
=============================

