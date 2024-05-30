# Normal flow

inline / block / inline-block

[Normal Flow - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Normal_Flow)

> If not using grid or flexbox, your elements display in normal flow. There are a number of layout methods that you can use to adjust the behavior and position of items when in normal flow.

[Layout](https://web.dev/learn/css/layout/#flow-layout)

## Inline block

`inline-block`It's still inline, but you can set margin and padding 

> Using inline-block gives you a box that has some of the characteristics of a block-level element, but still flows inline with the text.

from [https://web.dev/learn/css/layout/#flow-layout](https://web.dev/learn/css/layout/#flow-layout)

> If you have a document with some HTML marking up the content and view it in a browser, it will hopefully be readable. Headings and paragraphs will start on a new line, words display as a sentence with a single white space between them. Tags for formatting, such as em, do not break up the sentence flow. This content is being displayed in [Normal Flow](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flow_Layout), or Block Flow Layout. Each part of the content is described as “in flow”; it knows about the rest of the content and so doesn’t overlap.

If you work with rather than against this behavior, your life is made much easier. It is one of the reasons why [starting with a correctly marked up HTML document](https://brucelawson.co.uk/2018/the-practical-value-of-semantic-html/) makes a lot of sense, as due to normal flow and the inbuilt stylesheets that browsers have which respect it, your content starts from a readable place.

[How To Learn CSS - Smashing Magazine](https://www.smashingmagazine.com/2019/01/how-to-learn-css/#normal-flow)

[In Flow and Out of Flow - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flow_Layout/In_Flow_and_Out_of_Flow)

## Margin collapsing

> If two adjacent elements both have the margin set on them and the two margins touch, the larger of the two remains, and the smaller one disappears — this is called margin collapsing

from [https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Normal_Flow](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Normal_Flow)

[Mastering margin collapsing - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Model/Mastering_margin_collapsing)