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



const name = "hitesh"
const repoCount = 50;

console.log(`Hello my name is ${name} and my repo vount is ${repoCount}`);

const gameName = ne String('hiteshhc');
string is object in java script 

 console.log(gameName[0]);
 console.log(gameName__ptoto__)

console.log(gameName.length)//8
console.log(gameName.toUpperCase());

// kis  index par character 
console.log(gameName.charAt(2)); // t

// agar mujhe pata karna ho y kis position par hai 
console.log(gameName.indexOf("t"));

// most important method is slice ismen negative value nahi de sakte if dete hain yo ye ignore karke 0 se start kareg

const newString = gmaeName.subString(0,4);// hite include vale startindex yo endIndex -1


slice men keval negative vale de sakte hai 
const anotherString = gameName.slice(-8,4);


cosnt newStringOne = "  hitesh ";

isko fox katne ke liye hume string ke trim method.ko use karenge ye white space aur newline chartater par hi kam karta hai

console.log(newStringOne.trim());

const url = "hhtps://hotesh.com/hitehs chaoudhary

but browser change this https://hitesh.com/hitesh%20chaudhary

console.log(url.replace("%20", '-'))

you can ask is this thing is avilable

console.log(url includes("me"))

console.log(gameName.split("_"))

CLASS 6

const score = 400;
kai bat apko lagta hai ki ye data type number hi aap strictly define karna chahte ho 
const balance = new Number(100)
console.log(balance) // [Nimber : 100] 

console.log(balance.toString())
// 100 if you check typeof balance should so string type

console.log(balance.toFixed(2))

const otherNumber = 23.8996

console.log(otherNumber.toPrecision(3)); 23.9

const hindred = 1000000
console.log(hundreds .toLocaleString('en-IN'));


MAXvalue: Number

Math  most powerful  library

console.log(Math) all method and property you get and explore that 
console.log
Math.abs(4); //  4 either positive or negative
Math.round(4.6) // 5
Math.ceil(4.2)// 5
Math.floor(4.9)// 4
Math.min(4,3,5,8,2)
Math.max(4,3,5,8,2)

sabse jyada Math.random use hoti hai

its value is between 0 to 1

Math.random() 
(Math.random()*10) +1;

const min = 10;
const max = 20;
Math.floor(Math.random() * (max - min + 1)+min)

CLASS 7  Date 




let myDate = new Date();
console.log(myDate.toString());
myDate.toDateString()

myDate.toLocalString()
console.log(typeof myDate)

let myCreateDate = new Date (2023, 0, 23);
let myCreateDate =new Date  (2023, 0, 23, 5,3)
let myCreateDate = new Date ("2023-01-2023)
let myCreateDate = new Date ("01-14-2023")
console.log(myCreatedDate.toLocaleStrinh)

let myTimeStamp = Date.now();
console.log(myTimeStamp)
console.log(myCreatedDate.getTine());
console.log(Math.floor(Date.now()/1000))

CLASS 8
/) array
areay always in square bracet 
const myArr = [0,1,2,3,4,5];
the element of array string, number, boolean, aary, object , date etc
java script array are recylable
means we ca add remove value arrray after declaration array are  not assosiative 
we can access array using index
myArry[0]

they are shallow copy 


other method of declaration  of variable 

const myNewArry = new Aarray(1,2,3,4)

.push(6);
.put(); remove last element
.shift(); remove first element
.unshift(); add at the starting of array try yo aviod this only use if it's extremely required 

myArr.invludes(9);// boolean result
myArr indexOf(3);// result 1 or -1

const newArr = myawrr.join();
console.log(myArr);
console.log(newArr);
join bind array and convert , separated string

// slice, splice

console.log("A ", myaArr); 
slice return a sction of aaray
const myn1 = myArr.slice(1,3);
console.log(myn1);
console.log("B ", myArry);

const myn2 = myArr splice(1,3);
console.log("C", myArr)
consoole.log(myn2);
splice manupulate array 

array part 2

const marvel_hero = ["thor", "Ironman", "spiderman"];
const dc_hero = ["superman", "flash", "batman"];

marvel_heros.push(dc_heros);
console.log(marval_heros);

output :
["thor", "irin man", "spiderman", ["superman", "flash", "batman"]];

const allHeros = marvel_hero(dc_hero):

its give desire outpot :
["thor","iton man", "spider man", "flash", "batman"];

out most usefull operator is spread operator

const all_new_hero = [...marvel_hero, ...dc_hero];

const another_array = [1,2,3,[4,5,6],7,[6,7[4,5]]]

const real_another_array = another_array.flat(Infinity)

console.log(real_another_array)


console.log(Array.isArray("ram"); // false
console.log(Array.from("Ram")) // ["R", "a", "m"]
console.log(Array.from({name:"Ram"})); // its not able to convert this because  its don't understand which part to conevert in array key or value so we need to define to make array with key or with value 



may assume a situation 

let score1=100;
let score2=200;
console.log(Array.of(score1,scor2):;// [100,200]

// object
- singleton : vonstrutor se bana hua 
- jab hum literal se banate hai to singlton nahi banta
- jab hum constrtur se banate hai to singleton banta hai

const jsUser = {} // this is a object

const mySym =  Symbol("key1")
const jsUser ={
    name: "Ram",
    age:18,
     mySym: "myket1" // this wrong way to making key to symbol
    [mySym]:"mykey1" // this is the right way
    email: "ram@gmail com",
    isLogin:flase,
    lastLoginDays: ["Monday", "Saturday"],
    "full name": " Ram Gupta "
} // key always treat by system as string 
console.log(jsUser.name); // ram
console.log(jsUser[name]) // error when you try to access object property on braket need to abbd "' mark so system  understand its object value because we accessing array indexing also in bravket

console.log(jsUser["name"]) // this is right way
console.log(jsUser."full Name")// if define a vale this wat in object you cant access this way

console.log(jsUser["full name"]); this is the write way
console.log(jsUser.mySym)// its not work symbol also need access in double qoute 
console.log(typeof jsUser.mySym)// 
console.log(jsUser[mySym]);// this the right way



if you want yo lock an vaue of object then you need a freez method to apply object and define the vaue to be freezed.

Object.freez(jsUser)
jsUser.name="ram";

JsUser.greeting = function (){

    consolemlog("Hello js user ");
}

console.log(jsUser.greeting()) // Hello Js user
console.log(jsUser.greeting)// [Function (anonymous)]
jsUser.greetingTwo= function (){
    console.log("Hello Js user, $(this.name))
}






const tinderUser = {};

user.id = 1;
user name = "ram";

console.log(user);

const realUser = {
    email: "ram@gmail.com",
    fullname:{
        userFullName:{
        fname: "om",
        lname:"gupta"
        }
    }
}
optional chainin and chaining
console.log(realUser.fullname.userFullName.fname)// chaining

// optional chaining use if obj property not exist then we use this 
console.log(realUser.fullName?.userFullBame.fname);

const obj1 = {1: "a" , 2:"b"}

const obj3 {obj1, obj2}//

const obj4= Object.assign({}obj1,obj2)// {} it's  use empty  object as source and other are target

// epread way

const obj5= {...obj1, ...obj2}

// for value comming from database
const user =[
    {
        id:1,
        name:"ram"
    },
    {
        id:2,
        name:"om"
    }
]
console.log(Object.keys(tinderUser))
console.log(Object.valuse(tinderUser))
console.log(Object entries(tinderUser))
console.log(tinderUser.hasOwnProperty('isLoggedIn')) // true and flase


// Function 

function sayMyName() {
    console.log("r");
}

function  add (n1,n2){
    console.log(n1+n2)
}
add(5,6)

hum ese variable ke andar bhi store kar dete hain

const result = add(3, 2);
console.log(result) // undefined because  ye function return kuchh bhi nahi kqr raha keval console.log kar raha hao

function  addNumber(num1, num2){
    console.log("ram");
    return num1 +num2;
}

const newResult = addNumber(4,7) ;
console.log(newResult); now its work result 11

aur kitne tarike se value linja sakti hai 

function showMessage(username){
    return `${username} just logged`
}

shiwMessage("ram"); // not display becUse its a return type so its not show in conaole log

show i need first store this in an variable or direct console log to this function 

console.log(showMessage("ram")
or
const displayName = showMessage("ram");

console.log(dispalyName);

function showNewUser(userName){
    if(userName===undefined){
       console.log("please enter user name");
       return;
    }
    return `${userName} just logged in`
}

or function showNewUser(userName){
    if (!userName){
        console.log("please enter user name ")
    }
    return `${userName} just logged in`
}

or function with default parameter function showNewUser(userName: "guest"){
 return `${userNamr} just logged`
}

function restOperator(...num1){
    return num1;
}
console.log(restOpertor(200,300,500))
 
 const userObj = {
    name:"ram",
    price:100
 }

 function handelObj(anyobj){
    consol.log(` user name is ¢{anyobj.name}` and price is ${anyobj.price})
 }
handelObj(user);

const myArray = [200,100,500,700]

function returnSecondValue(getArray){
    rety getArray[1]
}
 console.log(returnSecondArray(myArray));


 // scope 

 if(true){
    console.log("a")
 }

