# Boîtes et contenu : 

The CSS box model est une boîte qui s'enroule autour de chaque élément HTML. Ça consiste en : margins, borders, padding, et the content.

La largeur/ hauteur total d'un élément devrait être calculé comme ceci :

- width + padding + border = actual visible/rendered width of an element's box

- height + padding + border = actual visible/rendered height of an element's box

Ainsi padding et border sont inclus à l'intèrieur de la boîte : si on veut qu'un élément fasse 350px de large = ```width: 320px; padding: 5px; borders: 10px```

![](/Users/alicefabre/Desktop/Cours/HTML-CSS/Box.png)