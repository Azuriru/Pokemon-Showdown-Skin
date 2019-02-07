# Pokemon Showdown Skin
Custom Skin for Pokemon Showdown, activates on Dark Mode so you don't go blind on Light Mode.

## Preview 
![Reshiram Custom Skin](https://i.gyazo.com/efcf3536888fac72ca6dab03ace01c3a.png)

## Installation
* Download [Tampermonkey](https://tampermonkey.net/)
* Click "Create a new script..." on the Extension
* Paste this in
```
// ==UserScript==
// @name         Reshiram Skin 
// @namespace    https://play.pokemonshowdown.com/*
// @version
// @description
// @author       k_OS
// @match        https://play.pokemonshowdown.com/*
// @icon         https://www.serebii.net/pokedex-sm/icon/643.png
// @grant GM_addStyle
// @grant GM_getResourceText
// @resource    css  https://raw.githubusercontent.com/GameModerator/Pokemon-Showdown-Skin/master/Reshiram.css
// ==/UserScript==

GM_addStyle(GM_getResourceText('css'));
console.log('Reshiram CSS loaded!');
```
* Click File > Save when you are done
* Go to [Pokemon Showdown!](https://play.pokemonshowdown.com/)
* Enable "Reshiram Skin" in the Extensions
* Reload Pokemon Showdown! if the skin doesn't show.

## Updates
Usually, if I update this, updates won't show up for you. So here's what you do to set it to auto-update every time, all the time.
* Open Reshiram Skin on Tampermonkey, you can do this by holding down CMD / Ctrl and clicking the switch for Reshiram Skin on Pokemon Showdown!
* Go to Settings on the top right
* Under General, set Config mode to "Advanced"
* Scroll down to Externals and change the Update Interval to "always"
