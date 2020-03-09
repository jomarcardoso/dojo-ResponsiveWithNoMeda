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
