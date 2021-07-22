We can use `:where` selector for reseting default CSS styles. `:where` always has 0 specifity.
```css
:where(ul[class]) {
  list-style: none; /* reset for all ul's with class */
}

.list {
  list-style: square; /* keep squares for custom list */
}
```
