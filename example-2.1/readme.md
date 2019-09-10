![Example 2.1](https://raw.githubusercontent.com/denisnarush/sessions-examples/master/example-2.1/example-2.1.png)
### Push block to the right side
HTML:
```html
<div class="container">
  <any class="element"></any>
  <any class="element"></any>
  <any class="element element_side_right"></any>
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
  width: 16.5%;
}

.element_side_right {
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

<details><summary>SOLUTION</summary>
<p>

```css
.container {
  /* setting container display value to flex */
  display: flex;
}

.element_side_right {
  /* can make possibility apply margin from left side to auto */
  margin-left: auto;
}
```

</p>
</details>

