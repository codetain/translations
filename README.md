# translations

[![NPM version][npm-image]][npm-url]

i18n-compatible package with common translations that can be used in your applications right away.

## Installation

```
npm install @codetain/translations
```

or

```
yarn add @codetain/translations
```

## Usage
You can simply import translations to your project and mix them with your current translations. When you use i18next you can pass it to resources like this:

```
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


[npm-url]: https://www.npmjs.com/package/@codetain/translations
[npm-image]: https://img.shields.io/npm/v/validator.svg
