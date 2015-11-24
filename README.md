# Como criar meu próprio framework CSS?

![CSS Selectors](https://i.ytimg.com/vi/TveUPhu0Vwo/maxresdefault.jpg)

Seleciona qualquer elemento da árvore.
```css
* {
  padding: 10px 20px;
  color: tomato;
}
```
```html
<p>I'm a paragraph</p>
<span>I'm a span</span>
```
------------------------------------------

Seleciona qualquer elemento da árvore. *E*
```css
E {
  text-decoration: underline;
  color: orange;
}
```
```html
<h1>Workshop CSS</h1>
```

------------------------------------------

Seleciona um elemento com um atributo específico. *E[attr]*
```css
E[lang] {
  color: gray;
}
```
```html
<span lang="">Hello there!</span>
<span>Psiuuu!!!</span>
```

------------------------------------------

Seleciona um elemento que contém um atributo com um valor específico. *E[attr=value]*
```css
E[lang="pt-br"] {
  color: blue;
}
```
```html
<span lang="pt-br">Hello Marcelo!</span>
<span lang="en">Hello there!</span>
<span>Helllooooo!</span>
```

------------------------------------------

Seleciona um elemento cujo o valor do atributo "attr" é exatamente "value" ou contém o "value" entre espaços em branco
```css
E[name~=Marcelo] {
  color: red;
}
```
```html
<h1 name="José Marcelo">Marcelo Silva!</h1>
```
