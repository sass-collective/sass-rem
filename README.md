![Sass Rem](.repo/banner.png)

[![Version](https://flat.badgen.net/npm/v/@sass-collective/sass-rem)](https://www.npmjs.com/package/@sass-collective/sass-rem)
[![Download](https://flat.badgen.net/npm/dt/@sass-collective/sass-rem)](https://www.npmjs.com/package/@sass-collective/sass-rem)
[![License](https://flat.badgen.net/npm/license/@sass-collective/sass-rem)](https://www.npmjs.com/package/@sass-collective/sass-rem)

## Introduction

Generate rem value.

## Install

    npm install @sass-collective/sass-rem --save

## Usage

### Module System

#### Sass

    @use "@sass-collective/sass-rem"

    // Function

    body {
        font-size: sass-rem.rem(16);
    }

    // Mixin

    body {
        @include sass-rem.rem(16);
    }

#### CSS

    body {
        font-size: 1rem;
    }

### Legacy @import

#### Sass

    @import "@sass-collective/sass-rem"

    // Function
    
    body {
        font-size: sass-rem(16);
    }

    // Mixin

    body {
        @include sass-rem(16);
    }

#### CSS

    body {
        font-size: 1rem;
    }
