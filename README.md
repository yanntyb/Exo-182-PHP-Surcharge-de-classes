Consignes :

- Vous allez créer une nouvelle classe appelée "sorcier", vous la placerez dans un fichier appelé sorcier.php dans le dossier classes
- Cette classe va hériter de la classe personnage
- Vous allez surcharger le constructeur de la classe sorcier pour que le constructeur ait exactement le même comportement
 que le constructeur de la classe personnage
 - a la suite de la surcharge du constructeur, vous définirez les propriétés x et y à 125
 - sur index.php, vous allez créer une nouvelle instance de princesse, une nouvelle instance de sorcier et tester
 les différentes valeurs de ces instances.





Théorie :

Lors de l'héritage d'une classe, certaines méthodes ne sont pas automatiquement héritée, c'est le cas de la méthode magique
__construct() qui s'éxécute lorsqu'une classe est instanciée.

Dans l'exercice précédent, je vous ai demandé de créer une classe princesse qui hérite de la classe personnage, si vous avez
 essayé de l'instancier , certaines propriétés n'étaient pas définies.

Dans la classe princesse, j'ai réalisé une surcharge du constructeur, j'éxécute en réalité le constructeur de la classe
 mere puis je redéfini les propriétés qui doivent être différentes dans la classe princesse.

Faire cela m'évite de réécrire tout le constructeur dans les classes enfants, c'est trés utile surtout si le constructeur
de la classe mere contient beaucoup de lignes de code.

Pour accéder à la méthode parente à ma classe, j'ai utilisé l'opérateur de portée "::"

J'aurais également pu aussi ecrire personnage::__construct(), parent ici est un mot clef permettant de faire référence à
la classe mere

Il existe d'autres mots clefs, comme "self" par exemple, qui fait référence à la classe elle même.