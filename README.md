# translations

[![NPM version][npm-image]][npm-url] [![NPM downloads][npm-downloads-image]][downloads-url] [![MIT License][license-image]][license-url]

i18n-compatible package with common translations that can be used in your applications right away.

## Installation

`npm install @codetain/translations`

or

`yarn add @codetain/translations`

## Usage
You can simply import translations to your project and mix them with your current translations. When you use i18next you can pass it to resources like this:

```javascript
import { en, de } from '@codetain/translations';

const resources = {
  en: {
    translation: { ...en, ...yourTranslationsEN }
  },
  de: {
    translation: { ...de, ...yourTranslationsDE }
  }
};

i18n
  .use(initReactI18next)
  .init({
    resources
  });
```

## Contributing

Please follow the "fork-and-pull" Git workflow.

1. Fork the repo on GitHub
2. Clone the project to your own machine
3. Work on your fork
    1. Make your changes and additions
        - Most of your changes should be focused on `locales/` folder, `index.js` and/or `README.md` files.
    2. Add changes to README.md if needed
4. Commit changes to your own branch
5. **Make sure** you merge the latest from "upstream" and resolve conflicts if there is any
6. Repeat step 3(3) above
7. Push your work back up to your fork
8. Submit a Pull request so that we can review your changes

## Maintainers

- [norberdo](https://github.com/norberdo) - **Norbert Suski**
- [artuone83](https://github.com/artuone83) - **Artur Wozniak**

## License (MIT)

```
Copyright (c) 2020 Codetain <developers@codetain.com>

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```


[npm-url]: https://www.npmjs.com/package/@codetain/translations
[npm-image]: https://img.shields.io/npm/v/@codetain/translations
[downloads-url]: https://npmcharts.com/compare/@codetain/translations?minimal=true
[npm-downloads-image]: http://img.shields.io/npm/dm/@codetain/translations.svg?style=flat

[license-image]: http://img.shields.io/badge/license-MIT-blue.svg?style=flat
[license-url]: LICENSE
