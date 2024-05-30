# Multi column layout

also legacy (?) unlikely to come up

[Introduction to CSS layout - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Introduction#multi-column_layout)

> If you have a really long list of elements, such as a list of all of the countries of the world, it can result in a lot of scrolling and time wasted for a user. It can also create excess whitespace on the page. With CSS multicolumn, you can split this into multiple columns to help with both of these issues.

```css
<h1>All countries</h1>
<ul class="countries">
  <li>Argentina</li>
  <li>Aland Islands</li>
  <li>Albania</li>
  <li>Algeria</li>
  <li>American Samoa</li>
  <li>Andorra</li>
  …
</ul>
```

```css
.countries {
	column-count: 2;
	column-gap: 1em;
}
```

[Layout](https://web.dev/learn/css/layout/#multicolumn-layout)