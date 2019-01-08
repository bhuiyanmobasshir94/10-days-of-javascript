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

# oject contains properties and methods

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
