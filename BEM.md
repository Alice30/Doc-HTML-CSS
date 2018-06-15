# Documentation BEM :

- Block 

- Element `__`

- Modifieur `--`


Mettre des noms de classe en relation avec le parent :

``` html
<header class="header"> 
  <nav class="headerNav">
     <ul class="headerNav headerNav--xmax">
       <li class="headerNav__item">
	<a href= "/about class="headerNav__itemLink">A propos</a>
      </li>
      <li class="headerNav__item">
	<a href= "/home" class="headerNav__itemLink headerNav__itemLink--isActive">Accueil</a>
       </li>
      <li class="headerNav__item">
	<a href= "/account" class="headerNav__itemLink headerNav__itemLink--isDisabled">Compte</a>
       </li>
       
```

``` sass

$bptablet: 768px;
$bpdesktop: 1024px; 

@mixin bp(val) {
  @media (min-width : #{val}) {
    @content; 
  }
}

.headerNav {
	display: flex; 
	justify-content: space-between;
	@include bp($bptablet){
		flex-direction: column; 
  }
  
  & -- xmas {
  background: red; 
  }
  
  &__item {
  list-style: none; 
  }

  &__itemLink {
  text-decoration: none; 
  
  }
  
    &--isDisabled {
    color: grey; 
    }
    
    &--isActive {
    color: green; 
    }
    
```


