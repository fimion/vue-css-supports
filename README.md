# vuecssbug

> demo

This is a demo of `@supports` and `@media` being used in a scoped style in vue. 

The expected result (the text should be red in chrome on a screen above 1024px)is not what happens due to the fact that 
the scoped variable is not applied to the double nested class definition. the original rule is applied because it is more specific.

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
