# CSS Specificity

how to calculate a selector’s specificity

1. Inline style - 1 000
2. IDs - 100
3. Class, attributes, pseudo class - 10
4. Element and pseudo element - 1

> Specificity is one of the four distinct stages of the cascade, which was covered in the last module, on the [cascade](https://web.dev/learn/css/the-cascade/).

[Specificity](https://web.dev/learn/css/specificity/)

> **Specificity**

Once you understand the fact that source order matters, at some point you will run into a situation where you know that a rule comes later in the stylesheet, but an earlier, conflicting, rule is applied. This is because that earlier rule has a **higher specificity** — it is more specific, and therefore is being chosen by the browser as the one that should style the element.

As we saw earlier in this lesson, a class selector has more weight than an element selector, so the properties defined on the class will override those applied directly to the element.

Something to note here is that although we are thinking about selectors and the rules that are applied to the thing they select, it isn't the entire rule which is overwritten, only the properties which are the same.

This behavior helps avoid repetition in your CSS. A common practice is to define generic styles for the basic elements, and then create classes for those which are different. For example, in the stylesheet below we have defined generic styles for level 2 headings, and then created some classes which change only some of the properties and values. The values defined initially are applied to all headings, then the more specific values are applied to the headings with the classes.

> Let's now have a look at how the browser will calculate specificity. We already know that an element selector has low specificity and can be overwritten by a class. Essentially a value in points is awarded to different types of selectors, and adding these up gives you the weight of that particular selector, which can then be assessed against other potential matches.

The amount of specificity a selector has is measured using four different values (or components), which can be thought of as thousands, hundreds, tens, and ones — four single digits in four columns:

> 1. **Thousands**: Score one in this column if the declaration is inside a style attribute, aka inline styles. Such declarations don't have selectors, so their specificity is always 1000.

```html
<h1 style="color:blue;">A Blue Heading</h1>
```

> 2. **Hundreds:** Score one in this column for each ID selector contained inside the overall selector.

`#someId`

> 3. **Tens**: Score one in this column for each class selector, attribute selector, or pseudo-class contained inside the overall selector.

`.someClassName`

> 4. **Ones**: Score one in this column for each element selector or pseudo-element contained inside the overall selector.

Element selector eg `h1` , `img` etc...

`!important` overrides all of the above (?)

> Note: The universal selector (`*`), combinators (`+`, `>`, `~`, ' `` '), and negation pseudo-class (`:not`) have no effect on specificity.

from 

[Cascade and inheritance - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Cascade_and_inheritance#specificity_2)

specificity

[Specificity - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Specificity)

[Specifics on CSS Specificity | CSS-Tricks](https://css-tricks.com/specifics-on-css-specificity/)

[Understanding CSS: Selector Specificity](https://medium.com/@dte/understanding-css-selector-specificity-a02238a02a59#.prouihvri)

from 2015

CSS Specificity comic

[CSS Specificity](https://cssspecificity.com/)

comic

[Specifishity :: Specificity with Fish](http://specifishity.com/)

## specificity calculators

[Specificity Calculator](https://specificity.keegan.st/)

Specificity calculator

[CSS Specificity calculator | Polypane, The Browser for Developers and Designers](https://polypane.app/css-specificity-calculator/)

## Specificity boost

specificity hack form [web.dev/learn/css/specificity](http://web.dev/learn/css/specificity) podcast
Repeating same class name, will increase the score. Eg one class === 10 points, 4 times the same class === 40 points.

```css
.className.className.className.className {
	//
}
```

> Caution: If you find that you are needing to boost specificity like this frequently, it may indicate that you are writing overly specific selectors. Consider whether you can refactor your CSS to reduce the specificity of other selectors to avoid this problem.

from [https://web.dev/learn/css/specificity/](https://web.dev/learn/css/specificity/)