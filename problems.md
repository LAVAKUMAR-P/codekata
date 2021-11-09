Given 3 numbers A,B,C print 'yes' if they can form the sides of a scalene triangle else print 'no'.
Input Size : A,B,C <= 100000
Sample Testcase :
INPUT
3 4 5
OUTPUT
yes

const readline = require('readline');
const inp = readline.createInterface({input: process.stdin});
const userInput = [];
inp.on("line", (data) => {userInput.push(data);
    
});
inp.on("close", () => {
    //start-here
let Size=userInput[0].split(" ").map((ele)=> parseInt(ele));
if(Size[0]+Size[1]>Size[2] && Size[0]+Size[2]>Size[1] && Size[1]+Size[2]>Size[0]){
   console.log("yes");
}
else{
     console.log("no");
}
});

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Given 3 angles A,B,C find if they can be interior angles of a triangle.If they form an interior triangle for the given angle,print 'yes' otherwise print 'no'.
Input Size : 0 <= A,B,C <= 180

const readline = require('readline');
const inp = readline.createInterface({input: process.stdin});
const userInput = [];
inp.on("line", (data) => {userInput.push(data);
    
});
inp.on("close", () => {
    //start-here
let angle=userInput[0].split(" ").map((ele)=> parseInt(ele));
if(angle[0]+angle[1]+angle[2] ===180 && angle[0]!==0 && angle[1]!==0 && angle[2]!==0){
    console.log("yes");
}else{
    console.log("no");
}
});
 ----------------------------------------------------------------------------------------------------------------------------------------------------------------------
Given k sorted arrays of possibly different sizes, merge them and print the sorted output.
Input Size : N<=100
Example:
INPUT
k = 3
1 3
2 4 6
0 9 10 11
OUTPUT
0 1 2 3 4 6 9 10 11

const readline = require('readline');
const inp = readline.createInterface({input: process.stdin});
const userInput = [];
inp.on("line", (data) => {userInput.push(data);
    
});
inp.on("close", () => {
    //start-here

let merged=[]
for(let i=0;i<3;i++){
    numbers=userInput[i].split(" ").map((ele)=> parseInt(ele));
   merged=[...merged,...numbers]
}

merged.sort(function(a, b){return a-b})
console.log(merged.join(" "));


});
 
 
 
 
 
 
 
 
  
 
 
 
 
 
 
 
 
  
