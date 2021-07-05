# LOCAL STORAGE

- property that allows JavaScript sites and apps to save key-value pairs in a web browser with no expiration date.

- Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data.
  but have some problems.

  - Cookies are included with every HTTP request.
  - sending data un encrypted over the internet.
  - Cookies are limited to about 4 KB of data.

- HTML5 Storage or DOM Storage
  key/value pairs locally Unlike cookies, this data is never transmitted to the remote web server
- you can retrieve that data with the same key. The named key is a string
  Calling `setItem()` with a named key that already exists will silently overwrite the previous value. Calling `getItem()` with a non-existent key will return null rather than throw an exception.
  Calling `removeItem()` with a non-existent key will do nothing.
- limited to about 5MB and can contain only strings

```js
myStorage = window.localStorage;
console.log(myStorage);
```

| Methods              | Action                                                                                                               |
| -------------------- | -------------------------------------------------------------------------------------------------------------------- |
| Storage.key()        | When passed a number n, this method will return the name of the nth key in the storage.                              |
| Storage.getItem()    | When passed a key name, will return that key's value.                                                                |
| Storage.setItem()    | When passed a key name and value, will add that key to the storage, or update that key's value if it already exists. |
| Storage.removeItem() | When passed a key name, will remove that key from the storage.                                                       |
| Storage.clear()      | When invoked, will empty all keys out of the storage.                                                                |

```js
if (!localStorage.getItem("bgcolor")) {
  populateStorage();
} else {
  setStyles();
}

function populateStorage() {
  localStorage.setItem("bgcolor", document.getElementById("bgcolor").value);
  localStorage.setItem("font", document.getElementById("font").value);
  localStorage.setItem("image", document.getElementById("image").value);

  setStyles();
}

function setStyles() {
  var currentColor = localStorage.getItem("bgcolor");
  var currentFont = localStorage.getItem("font");
  var currentImage = localStorage.getItem("image");

  document.getElementById("bgcolor").value = currentColor;
  document.getElementById("font").value = currentFont;
  document.getElementById("image").value = currentImage;

  htmlElem.style.backgroundColor = "#" + currentColor;
  pElem.style.fontFamily = currentFont;
  imgElem.setAttribute("src", currentImage);
}
```

Examples From MDN
