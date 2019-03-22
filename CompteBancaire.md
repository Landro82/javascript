Reprenons le contexte des comptes en banque issu d'un précédent exercice. Un compte bancaire sera modélisé par une classe définie comme suit :

Une propriété titulaire initialisée par le constructeur.

Une propriété solde valant initialement 0.

Une méthode crediter() ajoutant le montant passé en paramètre (éventuellement négatif) au solde du compte.

Une méthode decrire() renvoyant la description du compte.

Ecrivez un programme qui crée 3 comptes bancaires, l'un appartenant à Alex, le deuxième à Clovis et le troisième à Marco. Stockez ces comptes dans un tableau.

Ensuite, le programme crédite 1000 € et affiche la description de chacun des comptes.

// Ajoutez votre code ici
```
class Comptes{
  construtor(titulaire){
    this.titulaire = titulaire;
    this.solde = 0;
  }
  //Methode crediter()
crediter(montant){
  this.solde += montant;
}
//Methode decrire()
decrire(){
  return `Titulaire ${this.titulaire} a un compte soldé á ${this.solde}`;
}
}
const compte1 = new Comptes("Alex");
const compte2 = new Comptes("Clovis");
const compte3 = new Comptes("Marco");
const myComptes = [];
myComptes.push(compte1);
myComptes.push(compte2);
myComptes.push(compte3);
// Crédite et décrit chaque compte
for(const compte of myComptes){
  compte.crediter(1000);
  console.log(compte.decrire());
}
```
/*Titulaire undefined a un compte soldé á NaN*/
 
```
class Comptes{
  constructor(titulaire){
    this.titulaire = titulaire;
    this.solde = 0;
  }
  //Methode crediter()
crediter(montant){
  this.solde += montant;
}
//Methode decrire()
decrire(){
  return `Titulaire ${this.titulaire} a un compte soldé á ${this.solde}`;
}
}
const compte1 = new Comptes("Alex");
const compte2 = new Comptes("Clovis");
const compte3 = new Comptes("Marco");
const myComptes = [];
myComptes.push(compte1);
myComptes.push(compte2);
myComptes.push(compte3);
// Crédite et décrit chaque compte
for(const compte of myComptes){
  compte.crediter(1000);
  console.log(compte.decrire());
}

```
