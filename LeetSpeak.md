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
