# Flex box

> if we add `display: flex` to the parent, the three items now arrange themselves into columns. This is due to them becoming *flex items* and being affected by some initial values that flexbox sets on the flex container. They are displayed in a row, because the initial value of `[flex-direction](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-direction)` set on their parent is `row`. They all appear to stretch to the height of the tallest item, because the initial value of the `[align-items](https://developer.mozilla.org/en-US/docs/Web/CSS/align-items)` property set on their parent is `stretch`. This means that the items stretch to the height of the flex container, which in this case is defined by the tallest item. The items all line up at the start of the container, leaving any extra space at the end of the row.

from 

[Introduction to CSS layout - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Introduction#flexbox)

[A Complete Guide to Flexbox | CSS-Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

```css
.my-element div {
 	flex: 1 0 auto;
}
```

> The flex property is a shorthand for flex-grow, flex-shrink and flex-basis. You can expand the above example like this:

```css
.my-element div {
 flex-grow: 1;
 flex-shrink: 0;
 flex-basis: auto;
}
```

[Layout](https://web.dev/learn/css/layout/#flexbox)

[Flexbox](https://web.dev/learn/css/flexbox/)

[Flexbox Cheatsheet](http://apps.workflower.fi/css-cheats/?name=flexbox)

[What Happens When You Create A Flexbox Flex Container? - Smashing Magazine](https://www.smashingmagazine.com/2018/08/flexbox-display-flex-container/)

[Everything You Need To Know About Alignment In Flexbox - Smashing Magazine](https://www.smashingmagazine.com/2018/08/flexbox-alignment/)

[Flexbox: How Big Is That Flexible Box? - Smashing Magazine](https://www.smashingmagazine.com/2018/09/flexbox-sizing-flexible-box/)