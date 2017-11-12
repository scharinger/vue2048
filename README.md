# Vue 2048

> Playing with vue while making a simple game.

Based on the vue-cli simple webpack boilerplate.


## Dependencies

https://github.com/vuejs/vue-touch

## TODO

Begin partly from start with the **tile approach** which keeps track of all tiles in a simple array, where each track has cords and value. The old **grid approach** makes it hard to make the game behave like the original.

```javascript
tiles = [{x:0,y:0,v:2},{x:1,y:0,v:2} ... ]
```
1. Use vue watchers to make transition effects on value changes.
1. Keep track of swype movements, keep in state.
    1. Use that info to add slide effects on tiles that are "updated". 
    1. Change slide method names to be more logical, true to real life.
1. Finish the movement function, each dir is diffrent, use the best. 

[Game rules](./src/readme.md) needed to be implemented better.

## Caveats

Using `overflow-y:hidden` to prevent the chrome android reload.

## Deploy to surge.sh

To deploy to my site.
``` bash
npm run deploy
```
same as:
``` bash
npm run build
surge C:\Users\Tim\Documents\Repos\2048\ 2048.scharinger.se
```

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build
```

For detailed explanation on how things work, consult the [docs for vue-loader](http://vuejs.github.io/vue-loader).
