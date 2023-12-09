# Vietnamese-Accent-Removal
> A lightweight Node.js library for removing Vietnamese accents and generating slugs from Vietnamese text. This library helps normalize Vietnamese text by removing diacritics and creating slugs suitable for URLs.

## Installation
```sh
npm i remove-accent-vietnamese
```

```js
<script type="text/javascript" src='https://cdn.jsdelivr.net/gh/kenproxx/remove-accent-vietnamese@main/script.js'></script>
```

# Usage
```js
// Copy code
const vietnameseAccentRemoval = require('remove-accent-vietnamese');

const text = "Xin chào Việt Nam!";

// Remove Vietnamese accents
const withoutAccents = vietnameseAccentRemoval.removeAccentVietnamese(text);
console.log(withoutAccents);
// Output: "Xin chao Viet Nam!"

// Remove Vietnamese accents and convert to lowercase
const lowercasedWithoutAccents = vietnameseAccentRemoval.removeAccentVietnameseToLowerCase(text);
console.log(lowercasedWithoutAccents);
// Output: "xin chao viet nam!"

// Generate slug from Vietnamese text
const slug = vietnameseAccentRemoval.makeSlug(text);
console.log(slug);
// Output: "xin-chao-viet-nam"

// Generate slug from Vietnamese text and convert to lowercase
const lowercasedSlug = vietnameseAccentRemoval.makeSlugToLowerCase(text);
console.log(lowercasedSlug);
// Output: "xin-chao-viet-nam"

```
# Functions
```js
removeAccentVietnamese(string) // string: Removes Vietnamese accents from the input string.

removeAccentVietnameseToLowerCase(string) // string: Removes Vietnamese accents and converts the input string to lowercase.

makeSlug(strInput, symbol) // string: Generates a URL-friendly slug from Vietnamese text.

makeSlugToLowerCase(strInput, symbol) // string: Generates a URL-friendly slug from Vietnamese text and converts it to lowercase.

// param symbol: The symbol used to separate words in the slug. Default is "-".
```

# Contribution

>Feel free to use and contribute to this open-source project. If you encounter any issues or have suggestions, please open an issue on GitHub.