With a few simple properties in a parent element we can achieve several layouts without touching the children.

try changing `.container`

```css
.container {
  display: grid;
  grid-template-columns: 100px 100px 100px;
}
```

Columns are explicit and the rows are implicit

```css
.container {
  display: grid;
  grid-template-columns: 100px;
  grid-template-rows: 100px;
  grid-gap: 8px;
}
```

Gap goes between tracks

Takes many properties

```css
.container {
  display: grid;
  grid-template-columns: 300px auto;
  grid-template-rows: 100px;
  grid-gap: 8px;
}
```

New unit called fr

```css
.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 100px;
  grid-gap: 8px;
}
```

Same for row

```css
.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr;
  grid-gap: 8px;
}
```

`repeat()`

```css
.container {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-template-rows: repeat(4, 1fr);
  grid-gap: 8px;
}
```
