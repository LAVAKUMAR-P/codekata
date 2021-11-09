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
 
 
 
 
 
 
 
 
 
  
 
 
 
 
 
 
 
 
  
