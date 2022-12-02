// get the numbers into an array

const fs = require('fs');
var file = []; 

// Turn the provided array into individual strings within an array then console log length of array
file = String(fs.readFileSync("day2.txt", {encoding: 'utf8'})).split("\n");
console.log(`Data array contains ${file.length} items.`);

// find unique intems in the array to determine all possible outcomes then console log
function onlyUnique(value, index, self) {
    return self.indexOf(value) === index;
}

var unique = file.filter(onlyUnique);
console.log(unique);

// switch statement to run through each array item and check it against 
var total = 0
    
for (let i in file){

switch(file[i]){
    case ('A Z'):
        console.log(i);
        total += 7;
    case ('A X'):
        console.log(i);
        total += 3;
        break;
    case 'C X':
        console.log(i);
        total += 0;
        break;
    case 'B X':
        console.log(i);
        total += 8;
        break;
    case 'A Y':
        console.log(i);
        total -= 2;
        break;
    case 'C Z':
        console.log(i);
        total += 3;
        break;
    case 'B Z':
        console.log(i);
        total -= 1;
        break;
    case 'C Y':
        console.log(i);
        total += 9;
        break;
    case 'B Y':
        console.log(i);
        total += 3;
        break;
    default:
        break;
     }
    }


console.log(file);
console.log(total);
if (total > 0){
    console.log(file);
    console.log(`The winning number is ${total}.`);
} else{
    console.log('Fix your code.');
}
    // A Rock 
    // B Paper
    // C Scissors
    // X Rock
    // Y Paper
    // Z Scissors
    // 1 Rock
    // 2 Paper
    // 3 Scissors
    // 0 Win
    // 3 Draw
    // 6 Win
