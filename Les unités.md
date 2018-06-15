# Les unités :

### REM

C'est comme EM, mais c'est une mesure basée sur la taille de l'élément racine du HTML = "le navigateur". 
Par défaut, la taille du `<html>` est de 16 px, ce qui veut dire que `1rem = 16px`. Pour éviter de devoir faire des calculs afin de respecter les tailles relatives à votre maquette, vous pouvez ré-écrire cette font-size afin que `1 rem = 10px`.


```css
.html {
	font-size: 62,5%;
}

.mainTitle {
	font-size: 2.4rem;   (= 24px)
}

.cover {
	width: 32rem; (=320px)
}

```
  
### EM

Le EM à contrario du REM se base quant à lui sur la taille de son parent direct. (pas son grand parent) 


### VW

Pourcentage de largeur du viewport (le viewport est égal à 100 vw). 

### VH

Pourcentage de hauteur du viewport (le viewport est égal à 100 vh).

=> Le viewport représente la partie visible au sein de la fenêtre du navigateur. 

### FR

Fraction de l'espace restant (ex: Grid layout).

