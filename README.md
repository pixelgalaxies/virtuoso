# virtuoso

## Virtuoso is *another* Grid Library, but this one is built with the CSS Grid Module.

### Let's break it down. Here is a list of all the classes involved:
```
.all-12 

.sm-3-6-3 
.md-3-6-3 
.lg-3-6-3 

.sm-3-9 
.md-3-9 
.lg-3-9 

.sm-9-3 
.md-9-3 
.lg-9-3 

.sm-4-8 
.md-4-8 
.lg-4-8 

.sm-8-4
.md-8-4 
.lg-8-4 

.sm-eq 
.md-eq 
.lg-eq 
```

## That's it! Not too crazy right? Let's break it down even further:
### Looking at sm-3-9
#### the *sm* represents "small". This is the break point specification. An element prefixed with *sm* will make its children columns expand starting at 600px 

#### Screen sizes:
```
sm: expand at 600px 
md: expand at 900px 
lg: expand at 1200px

*note: elements viewed on a screen below 600px will be full width elements
```

### Now lets look at the 3-9 
#### Seeing two numbers tells us this element should expect two children elements. The first will be 1 fractional unit wide (1/4 of the available width), the second will be 3 fractional units wide (3/4 of the available width). The numbers used in Virtuoso are based off the 12 point grid system Bootstrap was built on. 

### .all-12, .sm-eq, md-eq, and .lg-eq
#### You probably noticed these classes and how they do not follow the above pattern. the all-12 class and the eq classes each have unique attributes that required different a different naming convention.

### .all-12
#### This class will be set to 1 fractional unit at all screen sizes meaning its child will have a width of 100% of the available space. 

### .sm-eq, md-eq, and .lg-eq
#### The eq stands for equal. You can have as many column children in a row with these class names and they will split the available space among themselves and all be an equal width. If you want 6 columns of equal widths, starting at medium screens, you simply need to create a row element with the class name *md-eq.* Then place 10 column elements in the row. They will auto-adjust and make sure each column has the same amount of space.


## That's it! Start building today!
