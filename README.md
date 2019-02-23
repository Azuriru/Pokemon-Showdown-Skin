# Pokemon Showdown Skin
Custom Skin for Pokemon Showdown, activates on Dark Mode so you don't go blind on Light Mode.

## Preview 
![Reshiram Custom Skin](https://i.gyazo.com/efcf3536888fac72ca6dab03ace01c3a.png)

## Installation
* Download [Tampermonkey](https://tampermonkey.net/)
* Click "Create a new script..." on the Extension
* Paste this in
```init
// ==UserScript==
// @name         Reshiram Skin
// @namespace    https://play.pokemonshowdown.com/*
// @version
// @description
// @author       k_OS
// @match        https://play.pokemonshowdown.com/*
// @icon         https://www.serebii.net/pokedex-sm/icon/643.png
// @grant        GM_addStyle
// @grant        GM_getResourceText
// @resource     css  https://raw.githack.com/GameModerator/Pokemon-Showdown-Skin/master/Reshiram.css
// ==/UserScript==

GM_addStyle(GM_getResourceText('css'));
console.log('Reshiram CSS loaded!');
```
* Click File > Save when you are done
* Go to [Pokemon Showdown!](https://play.pokemonshowdown.com/)
* Enable "Reshiram Skin" in the Extensions
* Reload Pokemon Showdown! if the skin doesn't show

### CSS
```CSS
@import url('https://raw.githack.com/GameModerator/Pokemon-Showdown-Skin/master/Reshiram.css')
```

### JS
#### Vanilla
```JS
var file = 'https://raw.githack.com/GameModerator/Pokemon-Showdown-Skin/master/Reshiram.css';
var link = document.createElement('link');
link.href = file;
link.type = "text/css";
link.rel = "stylesheet";
document.getElementsByTagName("head")[0].appendChild(link);
```

#### jQuery
```JS
$('head').append($('<link>', {
	'rel': 'stylesheet',
	'type': 'text/css',
	'href': 'https://raw.githack.com/GameModerator/Pokemon-Showdown-Skin/master/Reshiram.css'
}));
```

What else do ya need, man?
