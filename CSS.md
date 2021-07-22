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
