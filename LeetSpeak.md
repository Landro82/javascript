// Ajoutez votre code ici
```
 function convertirLettreLeet(lettre){
   let letterLeet = lettre;
   switch(lettre.toLowerCase()){
     case "a":
       letterLeet = "4";
       break;
     case "b":
       letterLeet = "8";
       break;
     case "e":
       letterLeet = "3";
       break;
     case "l":
       letterLeet = "1";
       break;
     case "o":
       letterLeet = "0";
       break;
     case "s":
       letterLeet = "5";
       break;
     case "p":
       letterLeet = "9";
       break;  
    case "r":
       letterLeet = "2";
       break;  
    case "t":
       letterLeet = "7";
       break;
   }
   return letterLeet;
 }
function convertirMotLeet(unMot){
  let motLeet =" ";
  for(const letter of unMot){
    motLeet += convertirLettreLeet();
  }
  return motLeet;
}
console.log(convertirMotLeet("Hello World!")); // "H3110 W0r1d!"
console.log(convertirMotLeet("Noob")); // "N008"
console.log(convertirMotLeet("Hacker")); // "H4ck3r"
```

Voici ma solution, mais je pense que tu as fait une erreur avec la valuer de r

```
function convertirLettreLeet(a){
   switch(a.toLowerCase()){
     case "a":
       return "4";
       break;
     case "b":
       return "8";
       break;
     case "e":
       return "3";
       break;
     case "l":
       return "1";
       break;
     case "o":
       return "0";
       break;
     case "s":
       return "5";
       break;
     case "p":
       return "9";
       break;  
    case "r":
       return "2";
       break;  
    case "t":
       return "7";
       break;
    default:
      return a;
   }
 }

function convertirMotLeet(unMot){
  let arr = unMot.split('');
  console.log(arr);
  let arr1 =[];
  for(let i = 0; i < arr.length; i++){
    arr1.push(convertirLettreLeet(arr[i]));
  }
  return arr1;
}
console.log(convertirMotLeet("Hello World!")); // "H3110 W0r1d!"
console.log(convertirMotLeet("Noob")); // "N008"
```
