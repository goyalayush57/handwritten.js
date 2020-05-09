<h1 align="center">Welcome to handwritten.js 👋</h1>
<p>
  <a href="https://www.npmjs.com/package/handwritten.js" target="_blank">
    <img alt="Version" src="https://img.shields.io/npm/v/handwritten.js.svg">
  </a>
  <a href="https://github.com/alias-rahil/handwritten.js/blob/master/LICENSE" target="_blank">
    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-yellow.svg" />
  </a>
</p>

> Convert text to handwritten!

# In your code:

## Installation

```bash
npm install --save handwritten.js
```

## Usage

```javascript
const handwritten = require('handwritten.js');
(async function(text) {
    let converted = await handwritten(text);
    if (handwritten) {
        converted.write("output.jpg");
    } else {
        console.log("The text was empty!");
    }
})("Hello, world!");
```

> Note: The function 'handwritten' returns a jimp object if the text is non-empty, else it returns a null value.

# Command line usage:

## Using without installation

```bash
npx lyrics-finder "dream theatre" "another day"
```

> Note: Use this method only if you plan to use lyrics-finder for one time, installing lyrics-finder globally (see-below) is recommended for multiple time usages.

## Installation

```bash
npm install lyrics-finder -g
```

> Note: **DO NOT** use sudo to install global packages! The correct way to do it is to tell npm where to install it's global packages: `npm config set prefix ~/.local`. Make sure `~/.local/bin` is added to `PATH`.

## Usage after installation
 
```bash
lyrics-finder "dream theatre" "another day"
```

# API

It takes two arguments, artist name and song name and returns the lyrics as a string if found, else it will return an empty string (if used in code). The CLI binary logs the lyrics on your console (stdout) if found, else it will log 'Not Found!'.

# Author

👤 **Rahil Kabani <rahil.kabani.4@gmail.com>**

# Show your support

Give a ⭐️ if this project helped you!

# 🤝 Contributing

Contributions, issues and feature requests are welcome!<br />Feel free to check [issues page](https://github.com/alias-rahil/lyrics-finder/issues).

# Lyrics-Finder

🏠 [Homepage](https://github.com/alias-rahil/lyrics-finder#readme)

# License

[MIT](https://github.com/alias-rahil/lyrics-finder/blob/master/LICENSE)
