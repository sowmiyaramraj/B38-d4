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

