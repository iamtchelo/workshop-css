# Como criar meu próprio framework CSS?

Quem nunca começou um projeto e fez os mesmos botões, tabelas, grids que você fez em outro projeto passado? Por quê você não cria o seu próprio framework e utiliza em seus projetos?

Não sou contra quem usa [Bootstrap](http://getbootstrap.com/), [Foundation](http://foundation.zurb.com/) ou outros frameworks que tem por ai, mas será que você realmente precisa deles?

# O que será abordado no workshop?

- Seletores
- Componentização

# Então vamos colocar a mão na massa?

![CSS Selectors](https://i.ytimg.com/vi/TveUPhu0Vwo/maxresdefault.jpg)

Antes de tudo, como escrevo código CSS?

![CSS Declarations](http://www.etsav.upc.edu/assignatures/portafoli/imatges/css.jpg)

Vamos conhecer um pouco dos seletores CSS, vamos abordar algumas coisas importantes aqui. Caso queira um material completo sobre isso, estude por aqui [CSS Reference - Codrops](http://tympanus.net/codrops/css_reference/)

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

Seleciona qualquer elemento da árvore. **E**
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

Seleciona um elemento com um atributo específico. **E[attr]**
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

Seleciona um elemento que contém um atributo com um valor específico. **E[attr="value"]**
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

Seleciona um elemento cujo o valor do atributo "attr" é exatamente "value" ou contém o "value" entre espaços em branco. **E[attr~="value"]**
```css
E[name~="Marcelo"] {
  color: red;
}
```
```html
<h1 name="José Marcelo">Marcelo Silva!</h1>
```

------------------------------------------

Seleciona um elemento cujo valor do atributo "attr" começa com a string "value". **E[attr^="value"]**

```css
span[value^="workshop"] {
  color: green;
}
```
```html
<span value="css workshop">Hellloooo!</span>
<span value="workshop css">Helllo!</span>
```

------------------------------------------

Seleciona um elemento cujo valor do atributo "attr" termina com a string "value". **E[attr$="value"]**

```css
span[value="css"] {
  color: yellow;
}
```
```html
<span value="css workshop">Hellloooo!</span>
<span value="workshop css">Helllo!</span>
```

------------------------------------------

Seleciona um elemento cujo valor do atributo "attr" contém a substring "value". **E[attr*="value"]**

```css
span[value="fa7"] {
  color: yellow;
}
```
```html
<span value="Workshop CSS na fa7">Workshop CSS na FA7</span>
```

------------------------------------------

Seleciona um elemento cujo valor do atributo "attr" é exatamente "value" ou começa com "value"

```css
span[lang|="pt"] {
  color: green;
}
```
```html
<span lang="pt">Text pt</span>
<span lang="pt-br">Text pt</span>
<span lang="pt br">Text pt</span>
```

------------------------------------------
