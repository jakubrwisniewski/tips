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

To nicely limit text to some length we can use `ch` unit - `1ch` is equal to single character length
```css
p {
  max-width: 75ch
}
```

---

To properly scale video we can use `aspect-ratio` property
```css
video {
  width: 100%;
  aspect-ratio: 16/9;
}
```

---

Make flex items to be spaced

```css
.flex {
  display: flex;
  gap; 10px; /* space between items set to 10px  */
}
```

---

Display multiline text without mapping newline characters to `<br>`
```css
section {
  white-space: pre-line;
}
```

---

Prevent text selection
```css
article {
  user-select: none;
}
```
