# Responsivo por natureza

Fazendo elementos responsivos sem usar media-queries

## Técnicas

```css
element {
  width: 100%;
  max-width: 300px;
}
```

```css
element {
  display: flex;
  flex-wrap: wrap;
}
```

Se o elemento for filho de flex

```css
element {
  width: calc(100% / 3);
  max-width: 100px;
}
```

Grid minmax

Fazer um wrapper do conteúdo com uma margem negativa.

Assemelha-se ao "grid-gap".

```html
<div>
  <div class="wrapper">
    <div>1</div>
    <div>2</div>
    <div>3</div>
  </div>
</div>
```

```css
.wrapper {
  margin: -10px;
}

.wrapper > * {
  margin: 10px;
}

@media (min-width: 1024px) {
  .wrapper {
    display: flex;
  }
}
```
