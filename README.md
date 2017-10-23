# typing-game
https://github.com/GwapTeam/self-introduction

## Overview
gakken educational self-introduction texts
Open html file using chrome.

### files
```
self-introduction
├── README.md
├── complete-self-introduction.html(Finished code)
├── extra-self-introduction.html(Extra code)
├── img/
└── self-introduction.html(First code)
```

### submodule
vendor file: https://github.com/GwapTeam/vendor

## Example
### clone
_Branch: `master`_
```bash
$ git clone -b master --recursive -j8 git@github.com:GwapTeam/self-introduction.git
```

_Branch: `development`_
```bash
$ git clone -b develop --recursive -j8 git@github.com:GwapTeam/self-introduction.git
```

_Branch: `feature`_
```bash
$ git clone -b feature --recursive -j8 git@github.com:GwapTeam/self-introduction.git
```

### pull submodule
```
$ git submodule foreach git pull origin master
```

<!-- Common Items -->

## Git rules

### branch
* master
    - Used for release
* develop
    - Used for release (operation confirmed)
* feature
    - Used for development (operation not confirmed)

The Teaching Material Creation Team check `development` branch and push it to` master` branch when judging it is usable.
The Developer always push the latest code to `feature` branch and push it to` development` branch on completion of the operation check.

### commit message
reference: https://qiita.com/KosukeSone/items/514dd24828b485c69a05

## Coding rules

### filename
_HTML, CSS: kebab-case_

* defalut : `original-filename.html`
* complete: complete-`original-filename.html`

_JS: snake case_

* default : `original_filename.js`
* complete: complete\_`original_filename.js`

_another files: snake case_

* img : `original_name.extension`

### HTML coding style

Use [HTML5](https://www.w3.org/TR/html5/)

Naming conventions: kebab-case
Tab Space         : 4space
String literal    : double quote

Case: Relative reference
```html
<!-- Bad -->
<script src=“./path/to/filename.js”></script>

<!-- Good -—>
<script src=“path/to/filename.js”></script>
```

### CSS coding style

Use [CSS3](https://developer.mozilla.org/ja/docs/Web/CSS/CSS3)

Naming conventions: kebab-case
Tab Space         : 4space

### JS coding style

Use [ECMAScript5](https://www.ecma-international.org/ecma-262/6.0/)

Tab Space     : 4space
String literal: double quote

Case: Variable declaration
```javascript
// Bad(ECMAScript6)
let   variable;
const constant;

// Good
var variable;
```

Case: anonymous function
```javascript
// Bad(ECMAScript6)
setTimeout(
  _ => console.log('left 1000ms'),
  1000
)

// Good
setTimeout(
  function () {
    console.log('left 1000ms');
    return true;
  },
  1000
)
```

reference: http://cou929.nu/data/google_javascript_style_guide/

