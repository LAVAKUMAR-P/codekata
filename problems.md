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
let yes
if(Size[0]+Size[1]>Size[2] && Size[0]+Size[2]>Size[1] && Size[1]+Size[2]>Size[0]){
   console.log("yes");
}
else{
     console.log("no");
}
});
 
 
 
 
 
 
 
 
 
  
