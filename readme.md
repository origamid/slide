## Slide Responsivo / Touch

Existem duas versões do slide, uma com controle de navegação e outra sem controles.

Adicione ao seu site o arquivo slide.js ou slidenav.js que estão dentro da pasta dist, assim como o arquivo slide.css.

```js
// código para o arquivo /dist/slide.js
// O primeiro seletor .slide, deve ser o elemento que envolve diretamente os slides.
// O segundo seletor deve ser um elemento a parte que envolve o .slide
const slide = new Slide(".slide", ".slide-wrapper");
slide.init();
```

```js
// código para o arquivo /dist/slidenav.js
// O primeiro seletor .slide, deve ser o elemento que envolve diretamente os slides.
// O segundo seletor deve ser um elemento a parte que envolve o .slide
// caso deseje controles acione os métodos addArrow e addControl
const slide = new SlideNav('.slide', '.slide-wrapper');
slide.init();
slide.addArrow('.prev', '.next');
slide.addControl('.custom-controls');
```