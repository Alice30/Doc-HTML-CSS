# Pseudo attribut ::after et ::before : 
  
Les pseudos attributs after et before sont essentiellement utilisés pour ajouter des éléments à votre DOM pour décorer sans que cela est un impact sur le référencement ou votre HTML. 
 
```html
  
  <section class="cover">
  	<h2 class="cover__title">Présentation</h2>
  </section>
 ```
 
 ```css
 
 .cover {
 	&__title {
	  font-size: 24px;
 	  color: #bbb;
	  text-align: center; 
 	  position: relative;
 	  &::before, 
	  &::after {
 	    content:'';    <-- à mettre important 
 		 position: absolute;
 		 top: 0;
 		 display: block; 
 		 background: green; 
 		 width: 50px; 
 		 height: 50px; 
 	  }
 		
 	  &::before {
 	  left: 0; 
 	  }
 		
 	  &::after {
 	  right: 0; 
 	  }				
 	}
 }

```	 

###**ATTENTION**
 
 * Il est obligatoire d'avoir un `content: ''` afin que vos after / before s'affichent. 
 * Vous pouvez leur donner une taille, une position (absolute par rapport à son parent