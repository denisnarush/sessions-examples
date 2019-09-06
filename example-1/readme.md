![Example 1](https://raw.githubusercontent.com/denisnarush/sessions-examples/master/example-1/example-1.png)
### Align block to the right side
HTML:
```html
<div class="container">
  <any class="element"></any>
</div>
```
CSS:
```css
.container {
  border: 3px dashed rgba(0, 0, 0, .2);
}

.element {
  background-color: #96C6FF;
  border: 3px solid #C2E2FA;
  height: 60px;
  width: 31.5%;
}
```
PRECONDITIONS:
- `div` can be any tag, representing `container`
- `any` can be any tag, representing `container`'s child `element`
- `container` has dynamic width
- `container` has dynamic height
- `element` has some width which can depend on his content or can have fixed value
- `element` has dynamic height
- don't use extra html
- don't use extra css selectors

___

<details><summary>SOLUTION 1</summary>
<p>

```css
/* 
 * when container not a block element:

 .container {
   display: block;
 }
*/

.element {
  /* setting element display value to block */
  display: block;
  /* can make possibility apply margin from left side to auto */
  margin-left: auto;
}
```

</p>
</details>

<details><summary>SOLUTION 2</summary>
<p>

```css
.container {
  /* setting container display value to flex */
  display: flex;
}

.element {
  /* can make possibility apply margin from left side to auto */
  margin-left: auto;
}
```

</p>
</details>
