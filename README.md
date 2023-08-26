# typescript-Assignment-2
The "typescript Assignment 2" GitHub repository contains TypeScript code and related files for the second assignment, demonstrating practical implementation and understanding of TypeScript programming concepts.



// Assignment for the week is:

//  - Create a function that takes an array, an index, and a value as parameters. 
// Inside the function, use the splice method to insert the value at the specified index in the array. 
// Return the modified array.

function aiv(array: number[], index: number, value: number){
    var addArray: number[] = array.splice(index, 0, value);
    return addArray
}
var array2 = [0, 0, 5];
var array3 = aiv(array2, 1, 10);
console.log(array3)

//  - Implement a simple shopping cart program using an array. Create functions to add items, remove items, 
// and update quantities using the splice method. Print the cart's contents after each operation

var myCart: [item: string, quantity: number][];
myCart = [["Pencil", 5], ["Pen", 3], ["Paper", 1]];
console.log(myCart); 

// add items
function addItems([]) {
    myCart.splice(3, 0, ["Rubber", 2], ["Colors", 1]);
}
var newCart: [] = [];
addItems(newCart);
console.log(newCart); 

// Remove items
function removeItem([]){
    myCart.splice(2, 1, ) ;
}
var afterRemoveItem: [] = [];
removeItem(afterRemoveItem);
console.log(afterRemoveItem); 

// update quantities
function updateQuantity([]){
myCart.splice([0][1], [0][1], ["Pencil",4]);
}
var cartUpdate: [] = [];
updateQuantity(cartUpdate);
console.log(myCart); 


//  - Write a program that uses a while loop to print the first 25 integers.

var first25: number = 0;
while(first25<26){
    console.log(first25);
    first25++
}

//  - Write a program that uses a while loop to print the first 10 even numbers.

var eNum: number = 0;
while(eNum < 21){
    if(eNum % 2 == 0){
        console.log(eNum);
    }
    eNum++
}

//  - Create a function that takes a positive integer as parameter and uses a while loop to calculate and 
// return the factorial of that number.

function calculateFactorial(aNum: number): number {

    var aFactorial: number = 1;

    while (aNum > 1) {
        aFactorial *= aNum;
        aNum--;
    }

    return aFactorial;
}

var fact = calculateFactorial(5);
console.log(fact);

//  - Write a program having an array of numbers if the number is negative it should remove the 
// negative number from the array.

function removeNegativeNumbers(negative: number[]): number[] {
    return negative.filter(number => number >= 0);
}

var negArray = [2, -5, 10, -3, 0, 8, -1];
var newArray = removeNegativeNumbers(negArray);

console.log("Original Array:", negArray);
console.log("Array without Negative Numbers:", newArray);

//  - Create a function that takes an array of numbers as parameter. Use a while loop to calculate and 
// return the sum of all the numbers in the array.
 
function sumArray(array1: number[]) {
var index: number = 0;
var sumArray: number = 0;
while (index < array1.length){
    sumArray += array1[index];
    index++
}
return sumArray
}

var actArray: number[] = [2, 3, 5, 1];
var getSumArray: number = sumArray(actArray);
console.log(`Sum of array value is = `, getSumArray)

//  - Implement a program that takes a list of temperatures in Celsius as input from the user. 
// Convert each temperature to Fahrenheit using the formula F = (C * 9/5) + 32 and store the 
// converted temperatures in an array. Use a while loop to perform the conversion for each temperature.



function tempC2F(tempC: number[] = []) {
var index = 0;
var tempInF: number[] = [];
while (index < tempC.length) {
    var tempF: number = (tempC[index] * 9/5) + 32;
    tempInF.push(tempF)
    index++
}   
return tempInF
}   

var tInF: number[] = [20, 37, 25, 19];
var listInF: number[] = tempC2F(tInF);
console.log(`List of temparature in H `, listInF)  


