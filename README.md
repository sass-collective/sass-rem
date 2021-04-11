![Sass Rem](.github/banner.png)

[![Version](https://flat.badgen.net/npm/v/@sass-collective/sass-rem)](https://www.npmjs.com/package/@sass-collective/sass-rem)
[![Download](https://flat.badgen.net/npm/dt/@sass-collective/sass-rem)](https://www.npmjs.com/package/@sass-collective/sass-rem)
[![Quality](https://flat.badgen.net/codacy/grade/0f9f3808eaa94177a98bd46b035410db)](https://app.codacy.com/gh/sass-collective/sass-rem)
[![License](https://flat.badgen.net/npm/license/@sass-collective/sass-rem)](https://www.npmjs.com/package/@sass-collective/sass-rem)

> **DEPRECATED:** this package has been moved to new reference in Sass Collective [monorepo](https://github.com/sass-collective/sass-collective/tree/master/packages/rem) `@sass-collective/rem`, use this package because the current repository is no more maintained.

## Introduction

Sass function & mixin to generate rem value.

## Install

    npm install @sass-collective/sass-rem --save

## Usage

### Function

```scss
rem($values);
```

### Mixin

```scss
rem($property, $values);
```

### Variables

| Names            | Values    |
| ---------------- | --------- |
| ``$baseline``    | 16        |

### Update default context in global

```scss
@use "@sass-collective/sass-rem" with (
    $baseline: 16
);
```

### Module System

```scss
@use "@sass-collective/sass-rem";

// Function

html,
body {
    // Single value
    font-size: sass-rem.rem(16);
    
    // Multiple values
    margin: sass-rem.rem(20 30);
}

// Mixin

html,
body {
    // Single value
    @include sass-rem.rem(font-size, 16);
    
    // Multiple values
    @include sass-rem.rem(margin, 20 30);
}
```

### Legacy @import

```scss
@import "@sass-collective/sass-rem";

// Function

html,
body {
    font-size: sass-rem(16);
    margin: sass-rem(20 30);
}

// Mixin

html,
body {
    @include sass-rem(font-size, 16);
    @include sass-rem(margin, 20 30);
}
```

### CSS

```css
html,
body {
    font-size: 1rem;
    margin: 1.25rem 1.875rem;
}
```
