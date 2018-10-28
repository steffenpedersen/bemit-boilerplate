# blepbemit 🎨

This is a boilerplate for using SCSS with [BEMIT](#bemit). 

That is a combination of the naming convention [BEM](#bem) and the [ITCSS](#itcss) architecture.

## BEM

BEM is a naming convention that makes the CSS easier to read and understand. It makes it easier to scale and generally more easy to work with. BEM is an abbreviation of the structure of the methodology. The elements of the structure is **B**lock, **E**lement and **M**odifier. The examples are tied to the ITCSS architecture.

### Block

This is a standalone entity that has its own meaning and purpose. The block is `.c-button`.

```scss
.c-button {
    display: inline-block;
    padding: 1em;
}
```

### Element

This should be a part of a block that has no standalone meaning and purpose. It should be semantically tied to its block. The element is `&__text`.

```scss
.c-button {
    display: inline-block;
    padding: 1em;
    
    &__text {
        font-size: 1em;
        font-weight: 400;
    }
}
```

### Modifier

This should be a flag on a block or an element. Here we are able to change appearance or behavior. The modifier is `&--bold`.

```scss
.c-button {
    display: inline-block;
    padding: 1em;
    
    &__text {
        font-size: 1em;
        font-weight: 400;
        
        &--bold {
            font-weight: 700;
        }
    }
}
```

One of the most important rules is, that you can't have an element inside an element and you can't have a modifier inside a modifier.

## ITCSS

## BEMIT
