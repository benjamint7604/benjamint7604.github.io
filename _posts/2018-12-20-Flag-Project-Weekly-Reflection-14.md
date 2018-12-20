---
layout: post
title: "Flag Project - Final Submission"
date: 2018-12-21
---

## Flag of Pakistan by Benjamin Ty

## Describe your program

-   I had designed a program to create a scalable flag of the country Pakistan.
-   For me I expect a practitioner as I had executed definitions in my code lines as well as going the extra expected mile of scaling it using the greatest common factor. I had executed my knowledge of knowing simple functions and creating functions and using test cases to figure out how to apply a scale factor.

<!--- Delete this comment and add your writing -->

## Current output

* * *
![Flag](/images/Final-Flag.png)
* * *

## Describe your process.

-  I had a couple of questions and struggles with trying to figure out how to scale the flag until the mini lesson that helped me understand how to use a scale factor more than I did before helping me in the process of scaling my flag.

<!--- Delete this comment and add your writing -->

## Explain your code.
* * *

```
;Main Parts/Details
(define size 5)
(define FLY(* size 120))
(define HOIST(* size 80))
```

* * *

-   I had posted this line of code specifically to show how I used a scale factor. As I define the word "size" as a variable that can be changed from 5 to 500 to an infinite amount of numbers. The other two functions known as "FLY" and "HOIST" which state that the variable is defined as "size" multiplied by a factor. I made the size 5 because if multiplied to the FLY and HOIST definition, it would equal to the given standard scale of a normal size of this kind of flag. Size is multipled to a factor that would make it equal to a perfect scale of a 600x400 flag size.
-   This code that I have here deals with the entire picture as it defines the scale factor to scale the entire picture and size the picture itself.

<!--- Delete this comment and add your writing -->

## Program code

```
;Pakistan Flag

;Main Parts/Details
(define size 5)
(define FLY(* size 120))
(define HOIST(* size 80))

(define pakistanGreen (make-color 0 40 0))
(define hotPink (make-color 255 105 180))
(define crecent (put-image(circle (* size 30) "solid" pakistanGreen) (* size  42) (* size 40) (circle (* size 30) "solid" "white")))
(define stars (rotate 20(star (* size 10) "solid" "white")))
(define background (rectangle (* size 180) (* size 120)"solid" "hotPink"))

;Main Flag
(define whiteBase (rectangle FLY HOIST "solid" pakistanGreen))
(define mainBase (put-image(rectangle (* size 30) (* size 80) "solid" "white") (* size 15) (* size 40) whiteBase))
(define crecentBase (put-image crecent (* size 80) (* size 40) mainBase))
(define starBase (put-image stars (* size 90) (* size 54) crecentBase))
(define pakistanFlag (put-image starBase (* size 90) (* size 60) background))

pakistanFlag
```
