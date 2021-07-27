### Create multiple dots
```js
'.'.repeat(5); // .....
```

---

### Prefixing stirng with characters
```js
"2".padStart(3, "0"); // 002
```

---

### Randomize array
```js
[].sort(() => Math.random() - 0.5)
```

---

### Filtering array for truthy values
```js
[false, 1, 0, '', 'cat', {}].filter(Boolean)
// output: [1, 'cat', {}]
```

---

### Access last element of array
```js
const list = ['a', 'b', 'c', 'd'];
list.at(-1); // 'd'
```

---

### Generate array with random numbers
```js
Array.from({ length: 1000 }, Math.random)
```

---

### Map array to array of numbers
```js
[5, '5', 3, 2, '80'].map(Number); // [5, 5, 3, 2, 80]
```

---

### Single called event listener
```js
element.addEventListener('click', () => null, { once: true });
```

---

### Smooth scrolling to element
```js
window.scrollTo({ top: 0, left: 0, behavior: 'smooth' });
```

---

### Checking if number is even
```js
const isEven = (number) => !(number & 1);
isEven(200); // true
isEven(201); // false
```

---

### Generate array of numbers
```js
Array.from({ length: 1000 }, (v, i) => i + 1); // [1, 2, 3, ...]
```

---

### Checking browser data saver

[https://developer.mozilla.org/en-US/docs/Web/API/NetworkInformation/saveData](https://developer.mozilla.org/en-US/docs/Web/API/NetworkInformation/saveData)
```js
if(navigator.connection.saveData) {
    // load compressed image
}
else {
  // load original image
}
```

---

### Get all controls of form
```js
const form = document.querySelector('form');
form.elements // HTMLFormControlsCollection []
```

---

### Checking if browser is online
```js
if(navigator.onLine) { // true | false
    // do something
}
 
// Update the online status changes
window.addEventListener('online',  callback);
window.addEventListener('offline', callback);
```

---

### Checking URL query parameters
```js
const urlSearchParams = new URLSearchParams(location.search);
const value = urlSearchParams.get('key');
```

---

### Generate seven last days
```js
[...Array(7).keys()].map(days => new Date(Date.now() - 86400000 * days))
```

---

## Alphabetical sorting
```js
["a", "z", "ą"].sort((a, b) => a.localeCompare(b)); // ["a", "ą", "z"]
```

---

### Validate url
```js
function validateUrl(url) => {
    try {
        new URL(url);
        return true;
    }
        catch(error) {
        return false;
    }
}
```

---

### Relative formatted difference between dates
```js
const rtf = new Intl.RelativeTimeFormat('en', { numeric: 'auto' });
const formatDays = (days) => rtf.format(days, 'day'); // "year", "quarter", "month", "week", "day", "hour", "minute", "second"

formatDays(10); // in 10 days
```
