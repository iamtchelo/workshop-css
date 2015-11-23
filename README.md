# Como criar meu próprio framework CSS?

# Seletores

```css
/* Qualquer elemento da árvore */
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

```css
/* Qualquer elemento com o nome E */
E {
  text-decoration: underline;
  color: orange;
}
```
```html
<h1>Workshop CSS</h1>
```

------------------------------------------

```css
/* Elemento E que contém o attributo "lang" */
E[lang] {
  color: gray;
}
```
```html
<span lang="">Hello there!</span>
<span>Psiuuu!!!</span>
```

------------------------------------------

```css
/* Elemento E cujo attributo "lang" é igual a "pt-br" */
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

```css
/* Element E cujo o valor do attribute "name" é exatamente "Marcelo" ou contém o nome "Marcelo" entre
espaços em branco */
E[name~=Marcelo] {
  color: red;
}
```
```html
<h1 name="José Marcelo">Marcelo Silva!</h1>
```
