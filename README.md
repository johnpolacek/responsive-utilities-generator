#Responsive Utilities Generator (SASS)

A SASS generator for creating responsive utility classes.

##How To Use

Open `responsive-utilities.scss`

Edit the utilityClasses mixin to define the responsive utilities you would like to include in your project.

In your CLI, run: 

```
sass responsive-utilities.scss responsive-utilities.css
```

To customize the breakpoints and breakpoint prefixes, pass in parameters to `responsiveUtilitiesGenerator()` in `responsive-utilities.scss`

For example, to use 5 breakpoints with em units:

```
@include responsiveUtilitiesGenerator(
  (0,30em,50em,75em,100em),    // breakpoints
  'em',               // breakpoint type 'px' or 'em'
  (xs-,s-,m-,l-,xl-)  // breakpoint prefixes
);
```

Then once again, run: 

```
sass responsive-utilities.scss responsive-utilities.css
```

##License
Author & copyright (c) 2015: [John Polacek](http://johnpolacek.com), Dual MIT & GPL license