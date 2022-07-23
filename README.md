# B38-d4
COMPARE 2 JSON OBJECT WITH SAME PROPERTY AND DIFFERENT ORDER
``````````````````````````````````````````````````````````
var obj1={name:"Person1",age:5};
var obj2={age:5,name:"Person1"};

if(  (obj1.name === obj2.name) &&( obj1.age ===obj2.age))
{

console.log( "true");
}
else
{
console.log( "false");
}


REST COUNTRTY 
flag
````
var request=new XMLHttpRequest();
request.open("GET","https://raw.githubusercontent.com/rvsp/restcountries-json-data/master/res-countries.json");
request.send();
request.onload=function()
{
    var result=JSON.parse(request.response);
   // console.log(result[122].currency);
   var nm=result.map((ele)=>ele.flag)
   nm.forEach(element => console.log(element));


}
NAME,REGION,SUB REGION,POPULATION
````````````````````````````````  
var request=new XMLHttpRequest();
request.open("GET","https://raw.githubusercontent.com/rvsp/restcountries-json-data/master/res-countries.json");
request.send();
request.onload=function()
{
    var result=JSON.parse(request.response);
   // console.log(result[122].currency);
   var nm=result.map((ele)=>ele.name)
   nm.forEach(element => console.log(element));

   var nm1=result.map((ele)=>ele.region)
   nm1.forEach(element => console.log(element));

   var nm2=result.map((ele)=>ele.subregion)
   nm2.forEach(element => console.log(element));

   var nm3=result.map((ele)=>ele.population)
   nm3.forEach(element => console.log(element));


}
