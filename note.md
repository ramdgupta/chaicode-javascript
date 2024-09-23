ki
Class1
Don't use var keyword
Only use let and const for variable declaration
Because issue of block scope and functional scope
let & const is block scope variable 
var is funcitonal scope variable
if any varaible either it's let,const or var is not in any bounded function in javascript file then it's parent object is window



CLASS 2
in old js class and module nahi the 
in new code are standarise 
when you use "use strict" it's means you are using all new syntax of Java script 
alert statement  alert(3+3)
in node js when we run its give us error because we are using node.js 
when we right in javascript file or browser alert open popup 
alert ko use karne ka tarika nod men hai par wo alag hai 
javascript engine hide in browser

console.log (3+3) console.log ("Hitesh")
it's not readable code show code should be raedeble so we need use semicolon after statment end 
if you enter line then error gone javascript inteligence auto under stood after enter there should be semicolon in hen your code statm nt is completed 

For documentation you need to r ad men mozila  but it's not original you need to follow ecma script documentation

Global object also is a datatype 
let name = "hitesh"; // string data type
let age =18; // integer type Data
let isLoogedIn=false;, // Boolean type 
let state  // means it's undefined 

// number => to power 53
// bigint  mostly we use for big number like stock data analysis 
// string => "" always use double code it's look good 
// Boolean => true/false
// nill => standalone value  it's special type of object in js 
if sever have issue and that why he send temprature value 0 then we don't prefer 0 as outpot because temprature is not zero it's sever falt so we use that time value as null

// undefined=> 
// symbol > for making uniqueness 
// object 

ek special opertor hai typeof

typeof(null)
result is object it's a Java script can you say it's bug

typeof(undefined) result is type undefined 

Note class: 2

PREMITIVE DATA TYPE

// number : 2 to power 53
// bigint
// string
// Boolean
// null
// undefined 
// symbol

NON PREMITIVE DATA TYPE 

// object
// array


CLASS 3 : Conversion and Declaration  it's a nightmare topic in Java script 

as we assume score variable is 33
let score =33
may be this value come from form we don't know the type of value is cnumber or string as first we see the above variable we can assume it's a number some we don't know from where we getting these blvalue 

but value like that req.body then it's a nightmare 
const {score } = req.body;
above line we don't assume the type of value I s number or string or Boolean 

for to the type of this value we right a console log
console.log(typeof score);
console.log(typeof(score));
both are type is valid

suppose this 33 is like that "33"

console.log(score);

then resul is "33"

if you want this value should be number then we need type conversion 

so we declare a new variable and and perform type conversion operation we achive this using javascript prebuild class function 
let valueNumber = Number(score);
console.log(typeof valueNumber); // it's print number
console.log(valueNumber); // print 33

may be it's not come value like "33" may be value is "33abc" should this convert same as like 33 to number let's 
see 

let newScore="33abc";
let newValueNumber = Number(newScore);
consolelog(typeof newValuNumber); // it's print number 
when we check value it's show Nan
console.log(newValueNumber) // result Nan it's means not a number

suppose let score = true/false // typeof result show 1/0
suppose let score = null // typeof result 0
suppose let score = undefined // typeof result Nan
suppose let score ="Ram" // typeof result Nan

let check reverse conversion for number 1 and 2 

let isLoogedIn=1;
let booleanloggedIn = Boolean(isLoggedIn);

console.log(booleanloggedIn) // true 
 suppose we define a number we check is number conver in string or not 
let someNumber = 123
let string number = String(someNumber);
console.log(stringNumber); // 33
consolemlog(typeof stringNumber)// String


Note class 2 : Type conversion 

// "33" : 33 
// "33abc" : Nan
// true : 1
// false : 0
// undefined: Nana
// any string value : Nan
// null : 0
// 1 : true
// 0 : false
// empty string: false


CLASS - 4 OPERATION 

let value = 3;
let newValue= - value;
console.log(negValue) // -3
apko pata hai result kya hoga 

console.log(2+2);
console.log(2-2);
console.log(2*2);
console.log(2**2)
console.log(2/2);
console.log(2%2);


let see one scenario we combining two string operation 

let str1 = "ram";
let str2 = "gupta"
let str3 = str1 + str2;
console.log(str3); // ram gupta 


suppose this operation done in a string and a number we har result should be with + operator 
console.log("1" + 2); // 3 
console.log(2 + "1"); // 3
console.lo("2" > 1); 
console.log("02"> 1);

console.log(null > 0); // sometime Nan and some time 0 
console.log(!null == 0);
console.log(null>=0);


console.log(undefined  == 0);
console.log(undefined> 0);
console.log(undefined 0);


console.log("2" === 2);
these are comarision yo br avid in professional  vode but in interview  point its important 

Class 5

// two type memory stack(premitive) and Heap (reference)

Basic example lete hai

let myYouTubeName = "rdGupta";

let anotherName = myYouTubeName;

anotherName ="shubiOm";

vonsole.log(myYouTubeName);//rdGupta
vonsole.log(anotherName); shubhiName

let userOne = {
    email: "user@mail com",
    upi: "payupi@mail.com"
}
let userTwo = userOne;
userTwo.email = "ram@mail.com";

console.log(userOne.email); // ram@ mail.com
console.log(userTwo.email); // ram@mail.com











