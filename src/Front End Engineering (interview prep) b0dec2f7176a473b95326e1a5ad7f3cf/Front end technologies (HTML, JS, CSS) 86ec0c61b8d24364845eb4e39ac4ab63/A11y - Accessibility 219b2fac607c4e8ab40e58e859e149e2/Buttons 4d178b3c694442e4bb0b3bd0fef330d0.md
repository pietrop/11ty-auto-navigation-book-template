# Buttons

**TLD:** It's important to distinguish what the functional role of the element on the page is vs whether it needs to look like a button or a link based on your design requirements (eg from your design system).

To decide you should start with identifying the functional role of the element on the page. Then if the behavior is not consistent with the default look and feel, you should override the style of `button` or `a` accordingly.

- Use `button`(s) for
    - Primarily originally for submitting forms (via html)
    - Clicks within the page, eg functionalities, like modals, collapse etc..
    - eg use custom style to make it look like a link if needed by the design requirements or design system
- Use `a` for
    - navigation within pages
    - navigation within areas of a page eg anchor links
    - outwards links
    - eg use custom style to make it look like a btn if needed by the design

    # Examples

    ## React Material UI

    Eg in React Material UI Lib [https://material-ui.com/api/button/#component-name](https://material-ui.com/api/button/#component-name)

    There's an optional `href` props that turns the underlying element from `button` to `a` for outward facing links.

    > `href` `string` The URL to link to when the button is clicked. If defined, an `a` element will be used as the root node.

    ## Bootstrap

    Similarly in Bootstrap [https://getbootstrap.com/docs/5.0/components/buttons/#button-tags](https://getbootstrap.com/docs/5.0/components/buttons/#button-tags) 

    > Button tags
    The `.btn` classes are designed to be used with the `<button>` element. However, you can also use these classes on `<a>` or `<input>` elements (though some browsers may apply a slightly different rendering).
    When using button classes on `<a>` elements that are used to trigger in-page functionality (like collapsing content), rather than linking to new pages or sections within the current page, these links should be given a `role="button"` to appropriately convey their purpose to assistive technologies such as screen readers.

    ```html
    <a class="btn btn-primary" href="#" role="button">Link</a>
    <button class="btn btn-primary" type="submit">Button</button>
    <input class="btn btn-primary" type="button" value="Input">
    <input class="btn btn-primary" type="submit" value="Submit">
    <input class="btn btn-primary" type="reset" value="Reset">
    ```

    ### React Bootstrap

    and in React boostrap [https://react-bootstrap.github.io/components/buttons/#button-tags](https://react-bootstrap.github.io/components/buttons/#button-tags) 

    > Normally `<Button>` components will render a HTML `<button>` element. However you can render whatever you'd like, adding a `href` prop will automatically render an `<a />` element. 

    You can use the `as` prop to render whatever your heart desires. React Bootstrap will take care of the proper ARIA roles for you.

    So this in React

    ```html
    <>
      <Button href="#">Link</Button> <Button type="submit">Button</Button>{' '}
      <Button as="input" type="button" value="Input" />{' '}
      <Button as="input" type="submit" value="Submit" />{' '}
      <Button as="input" type="reset" value="Reset" />
    </>
    ```

    renders to HTML as

    ```html
    <div>
    	<a href="#" class="btn btn-primary" role="button">Link</a> 
    	<button type="submit" class="btn btn-primary">Button</button> 
    	<input type="button" class="btn btn-primary" value="Input"> 
    	<input type="submit" class="btn btn-primary" value="Submit"> 
    	<input type="reset" class="btn btn-primary" value="Reset">
    </div>
    ```

    ---

    > Navigation: If you want a user to navigate to a new page or to a different target on the same page, use an anchor element <a>.

    [Buttons & Links | Accessibility Guidelines](http://web-accessibility.carnegiemuseums.org/content/buttons/)

    # ❓unclear ❓

    There's example of tabs widget using either `button` and `a`.

    And it's unclear which one is the best practice approach?

    W3C uses `button`