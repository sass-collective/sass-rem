![Sass Rem](.repo/banner.png)

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/f969e08f85544251a4c63b418780e184)](https://app.codacy.com/gh/sass-collective/sass-rem?utm_source=github.com&utm_medium=referral&utm_content=sass-collective/sass-rem&utm_campaign=Badge_Grade_Dashboard)
[![Version](https://flat.badgen.net/npm/v/@sass-collective/sass-rem)](https://www.npmjs.com/package/@sass-collective/sass-rem)
[![Download](https://flat.badgen.net/npm/dt/@sass-collective/sass-rem)](https://www.npmjs.com/package/@sass-collective/sass-rem)
[![License](https://flat.badgen.net/npm/license/@sass-collective/sass-rem)](https://www.npmjs.com/package/@sass-collective/sass-rem)

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

body {
    // Single value
    font-size: sass-rem.rem(16);
    
    // Multiple values
    padding: sass-rem.rem(20 30);
}

// Mixin

body {
    // Single value
    @include sass-rem.rem(font-size, 16);
    
    // Multiple values
    @include sass-rem.rem(padding, 20 30);
}
```

### Legacy @import

```scss
@import "@sass-collective/sass-rem";

// Function

body {
    font-size: sass-rem(16);
    padding: sass-rem(20 30);
}

// Mixin

body {
    @include sass-rem(font-size, 16);
    @include sass-rem(padding, 20 30);
}
```

### CSS

```css
body {
    font-size: 1rem;
    padding: 1.25rem 1.875rem;
}
```
