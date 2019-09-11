### 5 Stars rating
PRECONDITIONS:
- do not use JavaScript code

___

<details><summary>SOLUTION - IE7+</summary>
<p>

```html
<div class="rating">
  <input type="radio" id="rating12_1" name="rating12" value="1">
  <label for="rating12_1"></label>
  <input type="radio" id="rating12_2" name="rating12" value="2">
  <label for="rating12_2"></label>
  <input type="radio" id="rating12_3" name="rating12" value="3">
  <label for="rating12_3"></label>
  <input type="radio" id="rating12_4" name="rating12" value="4" checked>
  <label for="rating12_4"></label>
  <input type="radio" id="rating12_5" name="rating12" value="5">
  <label for="rating12_5"></label>
</div>
```
```css

.rating{
  font-size: 0;
}

input[id]{
  display: none;
}

label,
input{
  border-radius: 700px;

  display: inline-block;
  vertical-align: middle;

  margin: 0;
  padding: 0;

  width: 50px;
  height: 50px;
}

input,
label,
input:checked{
  background: yellow;
}

input:checked ~ input,
input:checked + label ~ label{
  background: gray;
}
 ```

</p>
</details>

<details><summary>SOLUTION - Modern</summary>
<p>

```html
<div class="rating">
  <input type="radio" name="starts">
  <input type="radio" name="starts">
  <input type="radio" name="starts" checked>
  <input type="radio" name="starts">
  <input type="radio" name="starts">
</div>
```
```css
.rating{
  display: flex;
  font-size: 0;
}

input {
  -webkit-appearance: none;
  -moz-appearance: none;
}

input{
  margin: 0;
  padding: 0;

  width: 50px;
  height: 50px;
}

input,
input:checked{
  background-image: url('data:image/svg+xml;base64,PHN2ZyB2ZXJzaW9uPSIxLjEiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiIHg9IjBweCIgeT0iMHB4IiB3aWR0aD0iMjBweCIgaGVpZ2h0PSIyMHB4IiB2aWV3Qm94PSIwIDAgMjAgMjAiIGVuYWJsZS1iYWNrZ3JvdW5kPSJuZXcgMCAwIDIwIDIwIiB4bWw6c3BhY2U9InByZXNlcnZlIj48cG9seWdvbiBmaWxsPSIjRkZERjg4IiBwb2ludHM9IjEwLDAgMTMuMDksNi41ODMgMjAsNy42MzkgMTUsMTIuNzY0IDE2LjE4LDIwIDEwLDE2LjU4MyAzLjgyLDIwIDUsMTIuNzY0IDAsNy42MzkgNi45MSw2LjU4MyAiLz48L3N2Zz4=');
  background-position: center center;
  background-size: 100%;
  background-color: transparent;
  background-repeat: no-repat;
}

input:checked ~ input{
  filter: grayscale(100%);
}
```

</p>
</details>
