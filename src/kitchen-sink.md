---
title: 'Kitchen sink'
image: 'https://images.unsplash.com/photo-1556911220-bff31c812dba?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2035&q=80'
emoji: 🍳
order: 2
---

---
## Text

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi finibus mi vulputate, venenatis lorem sed, sodales mi. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec in eleifend nulla. 

Pellentesque egestas hendrerit libero, id sollicitudin eros rhoncus at. Integer mattis, mauris nec pulvinar vehicula, tortor mi condimentum leo, a faucibus nisl magna luctus odio. Etiam varius enim et purus pulvinar cursus. 

Nullam pharetra maximus tellus, eget dictum arcu sagittis quis. Nam at hendrerit eros. Sed vel ultrices lorem. Cras iaculis felis sapien, sed sagittis diam dignissim vehicula.


---

## Headers

# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6


---

## code

### Code blocks


```
console.log('hello world')
```


### syntax highlighting 
```js
console.log('hello world')
```


### Inline Code snippet

In a quam at `console.log('hello world')` nisi bibendum blandit vel at mi. 

---

## details/summary html tag

<details>
<summary>Find out more</summary>
Test details summary html tag
</details>

---

## link


In a quam at [my site](https://pietropassarelli.net) nisi bibendum blandit vel at mi. Quisque semper massa in est vulputate dictum.

 <details>
<summary>Code example</summary>

```markdown
In a quam at [my site](https://pietropassarelli.net) nisi bibendum blandit vel at mi. Quisque semper massa in est vulputate dictum.
```
</details>


Note that if your link starts with `https://`, this is configure to open it in a new tab.



### internal links

internal links don't have preceding `/`

[animals](animals)
[mammals](animals/mammals)
[Moby dick](Moby%20Dick)

<details>
<summary>Code example</summary>

```markdown
[animals](animals)
[mammals](animals/mammals)
[Moby dick](Moby%20Dick)
```
</details>

---

## List

### Unordered list

- Cras dictum eros ut commodo feugiat. 
- Vivamus urna lectus, consequat vel fermentum sed, 
- pellentesque ac tortor. 
- Vestibulum lacinia varius mauris eu hendrerit. 
- Duis facilisis nisi quis risus tristique pellentesque. 
- Aliquam a ex tellus. 
- Class aptent taciti sociosqu ad litora torquent per conubia nostra, 
- per inceptos himenaeos.

### Ordered list

1. Cras dictum eros ut commodo feugiat. 
2. Vivamus urna lectus, consequat vel fermentum sed, 
3. pellentesque ac tortor. 
4. Vestibulum lacinia varius mauris eu hendrerit. 
4. Duis facilisis nisi quis risus tristique pellentesque. 
5. Aliquam a ex tellus. 
6. Class aptent taciti sociosqu ad litora torquent per conubia nostra, 
7. per inceptos himenaeos.


---

## Quote

> Duis facilisis nisi quis risus tristique pellentesque. Aliquam a ex tellus. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Sed ac tempor tortor, ut lobortis erat. Vivamus gravida sem massa, ut lobortis neque consectetur sit amet. Morbi sed eros cursus, euismod tellus et, sollicitudin mi. Nam eu velit efficitur, consectetur mauris rutrum, ultrices odio.


---

## Images

### Regular markdown image
![Alt image text](https://images.unsplash.com/photo-1475727946784-2890c8fdb9c8?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=2724&q=80)

Image from [unsplash](https://unsplash.com/photos/fHXP17AxOEk)


<details>
<summary>Code example</summary>
Just a markdown image

```
![Alt image text](https://images.unsplash.com/photo-1475727946784-2890c8fdb9c8?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=2724&q=80)
```
</details>

###  markdown image with link
[![Alt image text](https://images.unsplash.com/photo-1510158105534-9b01f2462ce1?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=2700&q=80)](https://unsplash.com/photos/gHwDURuSafI)



<details>
<summary>Code example</summary>
A markdown image wrapped in a markdown link

```
[![Alt image text](https://images.unsplash.com/photo-1475727946784-2890c8fdb9c8?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=2724&q=80)](https://unsplash.com/photos/fHXP17AxOEk)
```
</details>



---

## Video

<video controls preload='auto' width='100%' height='auto' poster='' data-setup='{}'>
  <source src='https://www.w3schools.com/html/mov_bbb.mp4'  type='video/mp4' />
</video>

<details>
<summary>Code example</summary>

```html 
<video controls preload='auto' width='100%' height='auto' poster='' data-setup='{}'>
  <source src='https://www.w3schools.com/html/mov_bbb.mp4'  type='video/mp4' />
</video>
```

</details>


---

## YouTube

To embed youtube, you just need to place the youtube url in it's own line, thanks to pugin.

https://youtu.be/id-zyjjOplY


<details>
<summary>Code example</summary>

```
https://youtu.be/id-zyjjOplY
```
</details>

---

## Vimeo

To embed vimeo, you just need to place the vimeo url in it's own line, thanks to pugin.

https://vimeo.com/128057278


<details>
<summary>Code example</summary>

```
https://vimeo.com/128057278
```
</details>


---

## Twitter

You can also embed a tweet, by just placing the tweet url on it's own line in the markdown file.

https://twitter.com/pietropassarell/status/1417199007072497668


<details>
<summary>Code example</summary>

```
https://twitter.com/pietropassarell/status/1417199007072497668
```
</details>


---

## Highlight 

Duis facilisis nisi quis risus tristique pellentesque. Aliquam a ex tellus. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. <mark>Sed ac tempor tortor, ut lobortis erat.</mark> Vivamus gravida sem massa, ut lobortis neque consectetur sit amet. Morbi sed eros cursus, euismod tellus et, sollicitudin mi. Nam eu velit efficitur, consectetur mauris rutrum, ultrices odio.


<details>
<summary>Code example</summary>

```html
Duis facilisis nisi quis risus tristique pellentesque. Aliquam a ex tellus. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. <mark>Sed ac tempor tortor, ut lobortis erat.</mark> Vivamus gravida sem massa, ut lobortis neque consectetur sit amet. Morbi sed eros cursus, euismod tellus et, sollicitudin mi. Nam eu velit efficitur, consectetur mauris rutrum, ultrices odio.
```
</details>



---


## Markdown rich text editing 

**Aliquam a ex tellus.**      
_Sed ac tempor tortor, ut lobortis erat._     
~~Strikethrough~~  

<details>
<summary>Code example</summary>

```markdown
**Aliquam a ex tellus.**      
_Sed ac tempor tortor, ut lobortis erat._
~~Strikethrough~~ 
```
</details>


---


## Auto dark mode

If you switch your system to darkmode the site, will use the darkmode css.


![Auto dark mode exmaple]({{site.baseUrl}}/img/kitchen-sink/kitchen-sink-auto-dark-mode-example.png)