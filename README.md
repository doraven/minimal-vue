# minimal-vue

## My problem20190605

Katex has a method `katex.renderToString(rawStr, displayMode: boolean, macros:{})`

>`displayMode` is used to decide show this equation inline or between lines.
>
>`macros`: used to define custom macros. 
>
>>>eg. macors: {"\ce{}" : "abc"} can render `\ce{}` as "abc"

Now problems is : if you want to render a chemistry equation, import [mhchem plugin](https://github.com/KaTeX/KaTeX/blob/master/contrib/mhchem/mhchem.js), but nothing happens.

Could someone see my [HelloWorld.vue](https://github.com/doraven/minimal-vue/blob/master/src/components/HelloWorld.vue) and the javascript plugin above and help me out of this problem.

Sincerely thanks.

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your tests
```
npm run test
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
