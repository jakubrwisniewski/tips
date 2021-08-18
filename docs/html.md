### Automatic input clear button
Cross button with no effort which clear input field on when pressed
```html
<input type="search" />
```

---

### Colored mobile browser header
So far only Mobile Chrome in light mode
```html
<head>
   <meta name="theme-color" content="#d00">
</head>
```

---

### Starting numeric list from specific number
```html
<ol start="5">
  <li>Five</li>
  <li>Six</li>
</ol>
```

---

### Image poster for video
```html
<video poster="link-to-poster-image.jpg">
  ...
</video>
```

---

### Automatic downloading file instead previewing
```html
<a href="file.txt" download>
  Download
</a>
```

---

### Image lazy loading
It will load the image when `img` tag is close to visible viewport
```html
<img loading="lazy" src="image.png" />
```

---

### Autofocus input
```html
<input type="text" autofocus />
```

---

### Validate input value by regex
```html
<input type="text" pattern="\d{4}-\d{2}-\d{2}" /> <!-- Autovalidates input on submit to match numeric format like 2000-01-01 -->
```