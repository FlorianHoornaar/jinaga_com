---
title: "predicate"
---

## Syntax

```pikchr
//========== COMMON SETUP ===============

scale = 1.0
$r = 0.2in
linerad = 0.75*$r  //rouding of lines
linewid = 0.15  //length of lines
Z:box invisible

//========== Predicate ====================

move down 100%
move left until even with Z.w
right

circle wid 10%
arrow right 200%

oval "." bold fit
arrow
oval "suchThat" fit
arrow
C:oval "(" fit

arrow right then up 60% then right
oval "j.not" fit
arrow
oval "(" fit
arrow

X:[
     text "Function that returns a" italic
     box "condition" italic bold fit fill 0xbebada with n at last.s
  ]
Border: box width X.width height X.height*1.3 at X.c

arrow
oval ")" fit
arrow right then down 60% then right

D:oval ")" fit

arrow right from C.e then down 60% then right until even with X.w

Y:[
     text "Function that returns a" italic
     box "condition" italic bold fit fill 0xbebada with n at last.s
  ]
Border: box width Y.width height Y.height*1.3 at Y.c

arrow left from D.w then down 60% then left until even with Y.e <-
right
arrow right 200% from D.e
circle wid 10%
```

See [condition](../condition/)

[Full diagram](../)