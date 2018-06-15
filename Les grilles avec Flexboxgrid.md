## Les grilles avec Flexboxgrid

* [Documentation http://flexboxgrid.com/]

Responsive modifiers enable specifying different column sizes, offsets, alignment and distribution at xs, sm, md & lg viewport widths.

Grid = bien pour le layout, mais il faut toujours des media queries pour le contenu 

* div class="container"(normal) = largeur d'une div 
* div class="container-fluid" = 100% de la largeur de l'écran

On commence par déclarer 1 row qui peut contenir maximum de 12 colonnes.

col-xs-12 étant le nombre de colonnes=(largeur = fine) pour la plus petite taille d'écran (mobile). Puis plus le nbre de colonne diminue (plus elles élargissent) et donc la taille de l'écran augmente.

On peut faire des grilles DANS les grilles. 

```html
<body>
  <div class="container">
    <div class="row">
      <div class="col-xs-12 col-sm-8 col-md-6 col-lg-3">Hello 1</div>
      <div class="col-xs-12 col-sm-8 col-md-6 col-lg-3">Hello 2</div>
      <div class="col-xs-12 col-sm-8 col-md-6 col-lg-3">Hello 3</div>
      <div class="col-xs-12 col-sm-8 col-md-6 col-lg-3">Hello 4</div>
      <div class="col-xs-12 col-sm-8 col-md-6 col-lg-3">Hello 5</div>
      <div class="col-xs-12 col-sm-8 col-md-6 col-lg-3">Hello 6</div>
    </div>
  </div>

</body>
```

  
Grids facilitent la gestion de la mise en page et gèrent des conceptions asymétriques.
Flexbox est idéal pour aligner le contenu à l'intérieur des éléments. 
