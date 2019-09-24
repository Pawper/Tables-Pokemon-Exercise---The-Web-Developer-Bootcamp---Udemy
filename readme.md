# Using CSS to Style the Pokemon Table Exercise
The instructor of the course used styling attributes on the HTML tags of the table in his solution video, but he also highly discouraged this. I know CSS, so I gave a shot at making a CSS file. He did the style as follows:
```html
<table border="1">
```
First, the `<table>` and `<th>`/`<td>` elements are given a `boder-width` of `1px`:
```css
table, th, td {
  border-width: 1px;
}
```
Then, I looked at the styles rendered using the `border="1"` attribute and discerned that the table has a `border-style` of `outset`, while th/td elements have a `border-style` of `inset`:
```css
table {
  border-width: 1px;
  border-style: outset;
}
th, td {
  border-width: 1px;
  border-style: inset;
}
```
Finally, I looked up the default `border-color` for HTML (https://www.w3schools.com/cssref/css_default_values.asp) to see that the default is `gray`.
```css
table {
  border-width: 1px;
  border-style: outset;
  border-color: gray;
}
th, td {
  border-width: 1px;
  border-style: inset;
  border-color: gray;
}
```
Finally, I switched to the shorthand syntax.
```css
table {
  border: 1px outset gray;
}

th, td {
  border: 1px inset gray;
}
```
I gave images a `width` of `50px` as per his solution video.
```css
img {
  width: 50px;
}
```