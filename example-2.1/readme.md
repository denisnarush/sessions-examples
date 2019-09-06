![Example 2.1](https://raw.githubusercontent.com/denisnarush/sessions-examples/master/example-2.1/example-2.1.png)
### Push block to the right side
HTML:
```html
<div class="container">
  <div class="block"></div>
  <div class="block"></div>
  <div class="block block_side_right"></div>
</div>
```
CSS:
```css
.container {
  border: 3px dashed rgba(0, 0, 0, .2);
}

.block {
  background-color: #96C6FF;
  border: 3px solid #C2E2FA;
  height: 60px;
  width: 16.5%;
}

.block_side_right {
}
```
PRECONDITIONS:
- container width: any
- container height: any
- block width: any
- block height: any
- don't use extra html
- don't use extra css selectors
