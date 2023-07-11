# javascript
Employee tracking app
class EmployeeTracking{
    constructor(firstnames, lastnames, years ){
        this.firstnames = firstnames
        this.lastnames = lastnames
        this.years = years 
    }

}
let person1 = new EmployeeTracking("chituru", "emmanuel", 12)

let person2 = new EmployeeTracking("onwuchekwa", "chika", 10)

let person3 = new EmployeeTracking("chikezie", "chinedu", 5)

let workers = [person1, person2, person3]

EmployeeTracking.prototype.data = function data(){
return this.firstnames + " " + this.lastnames +" has worked in our company for "+ this.years + " years"
      
 }       
workers.forEach((track) => {
    console.log(track.data())
})





function getRecursive(nr) {
    
    if(nr > 0) {
        getRecursive(nr - 1)
        console.log(nr)
    }else{
        console.log("done with recursive")
    }
    console.log("ended function")
}
getRecursive(3)







 //creating a basic calculator that takes two numbers and one string value indicating an operation.
 let x = 6
 let y = 5
 let operator = "+"

 function addNumbers(x, y, operator){
     return x + y 
 }
     if(operator == "+" || "-"){
         let addition = x + y 
         
     }else{
         let substration = x - y
        
     }

 addNumbers(x, y, operator)





let numbers = x => console.log("one")

let value2 = y => console.log("two")


let value3 = a =>{
   console.log("three")
    numbers()
    value2()
} 
let value4 =() =>{
console.log("four")
    setTimeout(numbers, 0)
    value3()
}
value4()




class person{
    constructor(firstname, lastname, color){
        this.firstname = firstname
        this.lastname = lastname
        this.color = color
    }
    greet(){
        console.log("hi, there")
    }
}
    person.prototype.introduce = function(){
        console.log("hi, i'm", this.firstname)
    }
    
    let p = new person("chituru", "onwuchekwa", "green")
    p.introduce()
   console.log(p.firstname, "likes", p.color)
    





class Animal {
    constructor(species, sounds){
        this.species = species
        this.sounds = sounds
    }

    speak(){
        console.log(this.species + " " + this.sounds)
    }   
}
Animal.prototype.eat = function(){
    return this.species + " is eating" 
}
let dog = new Animal("dog", "barks")
let cat = new Animal("cat", "meows")
dog.speak()
cat.speak()
console.log(dog.eat())
console.log(cat)
console.log(dog)




let arr = []
let multiply = 8

for(let i = 0; i < 8; i++){
    let temp = []
    for(let j = 0; i < 8; j++){
        let multiplication = i * j
        
    }
    temp.push(multiplication)
        arr.push(temp)
}
console.table(arr)





/* A to-do list 
a welcome message
input the task to be done
set the time to accomplish the task
additional motivational words 

*/
const toDoList = []
const maximumTodos = 50

let welcome = () => {
    // we ask for the user's name//
    const askName = prompt('Kindly enter your name: ')
    return ("hello," + askName + "!")
}
// User inputs the list of activities to carried out by the user//
let addTodo = () => {
    let text = prompt('Enter activity: ')
    const time = prompt("set time  (YYYY-MM-DD HH:MM) ( )" )
                                       
    const todo = {
        text:text,
        time:time
    }
    // using the .push method to push the object values into the array, it will stored in the array
    toDoList.push(todo)
    }
    
   
    function displayTodoList(){
        for(const todo of ToDoList){
            return `-${todo.text} at ${todo.time}`
        }
    }
           
    

    /* we loop through the array using a for loop so the user can input any amount of tasks to be done and 
    returns the user"s tasks that is to be accomplished and time the user wants to accom-
    plish the task 
    */
    for(let i = 0; i < maximumTodos; i++){
        if(addTodo() > maximumTodos){
            return "limit exceeded"
        }else{
            return
        }
        
    }


    // we create a function to set an alarm to alert the user of the task that is to be accomplished
    
    function setAlarm(todo){
        const alarmTime = new Date (todo.time)
        const now = new Date()
        const difference = alarTime - now
        const milliseconds = difference * 1000

        window.setTimeout(() =>{
            return (`Alarm for ${todo.text}!`);
         }, milliseconds)

         for(const todo of toDoList){
             setAlarm(todo)
         }

        }
    




  welcome()
  addTodo()
  displayTodoList()
  setAlarm(todo)








const studentname = {david: 80,
                    vinoth: 77,
                    divya: 88,
                    isihitha: 95,
                    thomas: 68
                }
              
// calculating the average, 5 is the total number of items in the object
let average = ((80 + 77 + 88 + 95 + 68)/5)
console.log(average)

if(average > 90 ){
    console.log(" Grade: A")
}else if(average > 80){
    console.log("Grade: B")
}else if(average > 70){
    console.log("Grade: C")
}else if(average > 60){
    console.log("Grade: D")
}else{
    console.log("Grade: F")
}


    

