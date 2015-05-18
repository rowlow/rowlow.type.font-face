# rowlow.type.font-face

A font-face wrapper to quickly define custom fonts for ROW LOW framework

## Install

```
    bower install --save rowlow.type.font-face
```


## Functions

```
    /**
     * $font-name Name of the font-family
     * $class-name The name of the class that will be generated
    **/
    rowlow-font-face($font-name, $class-name, $file, $fallback: sans-serif, $weight: normal, $style: normal)
```


## Usage

### SCSS
```
    /* Set modules namespace (optional) */
    $rowlow-font-face-namespace: "namespace-";

    @import "bower_components/rowlow.type.font-face/main.scss"

    @include rowlow-font-face('Futura Medium', 'futura-medium', '../fonts/futura-medium/futura-medium');

    <!-- preferred method -->
    h1{
        @extend .font-face--futura-medium;
    }

    <!-- alternate method -->
    h1{
        font-family: "Futura Medium", sans-serif
    }

```

### HTML
```
    <h1 class="font-face--futura-medium">This is Futura</h1>
```