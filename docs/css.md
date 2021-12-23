# CSS

### Better CSS reset
We can use `:where` selector for reseting default CSS styles. `:where` always has 0 specifity.
```css
:where(ul[class]) {
  list-style: none; /* reset for all ul's with class */
}

.list {
  list-style: square; /* keep squares for custom list */
}
```

---

### Limit text length by characters count
To nicely limit text to some length we can use `ch` unit - `1ch` is equal to single character length
```css
p {
  max-width: 75ch
}
```

---

### Video scaling by aspect ratio
To properly scale video we can use `aspect-ratio` property
```css
video {
  width: 100%;
  aspect-ratio: 16/9;
}
```

---

### Make flex items to be spaced

```css
.flex {
  display: flex;
  gap: 10px; /* space between items set to 10px  */
}
```

---

### Display multiline text without mapping newline characters to `<br>`
```css
section {
  white-space: pre-line;
}
```

---

### Prevent text selection
```css
article {
  user-select: none;
}
```

---

### Change color of text selection
```css
::selection {
  background-color: deeppink;
  color: white;
}
```

---

### Alternative for position `top` `left` `right` `bottom` properties
```css
div {
  position: absolute;
  inset: 1rem;
}
aside {
  position: relative;
  inset: 1px 2px 3px 4px;
}
```

---

### Light / Dark mode support
```css {
@media (prefers-color-scheme: dark) {
  body {
    background: black;
    color: white;
  }
}
@media (prefers-color-scheme: light) {
  body {
    background: white;
    color: black;
  }
}
```

---

### Trimming text
```css
.text {
  width: 100px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}
```

---

### Limit visible lines of text
```css
.box {
    -webkit-line-clamp: 2; /* how many lines to show */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    overflow: hidden;
}
```

---

### Arrows in pure CSS
```css
.arrow-up {
	width: 0; 
	height: 0; 
	border-left: 5px solid transparent;
	border-right: 5px solid transparent;
	border-bottom: 5px solid black;
}

.arrow-down {
	width: 0; 
	height: 0; 
	border-left: 20px solid transparent;
	border-right: 20px solid transparent;
	border-top: 20px solid red;
}

.arrow-right {
	width: 0; 
	height: 0; 
	border-top: 30px solid transparent;
	border-bottom: 30px solid transparent;
	border-left: 30px solid green;
}

.arrow-left {
	width: 0; 
	height: 0; 
	border-top: 10px solid transparent;
	border-bottom: 10px solid transparent; 
	border-right:10px solid blue; 
}
```

---

### Custom scrollbar style
```css
::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-track {
  background: pink;
  border-radius: 12px;
}

::-webkit-scrollbar-thumb {
  background: deeppink;
  border-radius: 12px;
}
```

---

### Center content
```html
<div class="container">
  <div>center</div>
</div>
```
```css
/* Using grid */
.container {
  display: grid;
  place-content: center;
  height: 100vh;
}

/* Using flex */
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100vw;
  height: 100vh;
```
