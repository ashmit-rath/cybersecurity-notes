# JavaScript Basics (Web Interaction)

JavaScript is used to make websites interactive.

--------------------------------

## Output

console.log("Hello")

alert("Hello")

--------------------------------

## Variables

let name = "Ash"
const age = 18

console.log(name)
console.log(age)

--------------------------------

## User Input

let user = prompt("Enter username")
console.log(user)

--------------------------------

## Button Interaction

HTML:
<button onclick="clickMe()">Click</button>

JavaScript:
function clickMe(){
    alert("Button clicked")
}

--------------------------------

## Change Page Content

HTML:
<p id="text">Hello</p>

JavaScript:
document.getElementById("text").innerHTML = "Changed"

--------------------------------

## Form Input Example

HTML:
<input id="username">
<button onclick="getUser()">Submit</button>

JavaScript:
function getUser(){
let user = document.getElementById("username").value
console.log(user)
}

--------------------------------

## If Condition

let age = 18

if(age >= 18){
console.log("Adult")
}else{
console.log("Minor")
}

--------------------------------

## Loop

for(let i=0;i<5;i++){
console.log(i)
}

--------------------------------

## Useful for Security Testing

Check page title
document.title

Get cookies
document.cookie

Redirect page
window.location = "http://example.com"

--------------------------------

## Event Listener

document.addEventListener("click", function(){
console.log("Clicked")
})
