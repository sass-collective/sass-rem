# Sass Rem

Generate rem CSS value.

## Install

    npm install @sass-collective/sass-rem --save

## Usage

### Global @import

#### Sass

    @import "@sass-collective/sass-rem"

    body {
        font-size: sass-rem(16);
    }

#### CSS

    body {
        font-size: 1rem;
    }

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
