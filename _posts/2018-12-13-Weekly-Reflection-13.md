---
layout: post
title: "Benjamin Ty, AFSE Student, Week #12,"
date: 2018-12-07
---

# Code
```
;Pakistan Flag

;Main Parts/Details
(define size 5)
(define FLY(* size 120))
(define HOIST(* size 80))

(define pakistanGreen (make-color 0 40 0))
(define hotPink (make-color 255 105 180))
(define crecent (put-image(circle (* size 30) "solid" pakistanGreen) 210 200 (circle (* size 30) "solid" "white")))
(define stars (rotate 20(star (* size 10) "solid" "white")))
(define background (rectangle (* size 180) (* size 120)"solid" "hotPink"))

;Main Flag
(define whiteBase (rectangle FLY HOIST "solid" pakistanGreen))
(define mainBase (put-image(rectangle (* size 30) (* size 80) "solid" "white") 75 200 whiteBase))
(define crecentBase (put-image crecent (* size 80) (* size 40) mainBase))
(define starBase (put-image stars (* size 90) (* size 54) crecentBase))
(define pakistanFlag (put-image starBase (* size 90) (* size 60) background))

pakistanFlag
```
# Flag
![Flag Screenshot](/images/flag2.png)

# Reflection
Some questions I've had over the past few days are how can one scale the position of the small details of ones flag. As well as if this is possible to scale the position by a common factor. I had barely any challenges besides scaling and I look forward to next weeks continuation in helping with scaling our flags to fit with one factor.
