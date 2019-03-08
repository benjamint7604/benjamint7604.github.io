---
layout: post
title: "Video Game Project"
date: 2019-3-8
---
## Video Game Project (Club Penguin Revival)

- This project is just my own video game based on the information I've learned in class about the manipulation of a character applying to the parameters for this game to function.

## My Code
```
(EXAMPLE (line-length 20 10) (- 20 10))
(EXAMPLE (line-length 10 20) (- 20 10))

(define (line-length a b)Collide takes in the distance between these objects and produces whether or not they are colliding based on if the range value is within the parameters of a specified amount. In the function, used as an example, this takes the coordinates and checks to see whether or not they are within 50 units of each other.
  (cond
    [(> a b) (- a b)]
    [else (- b a)]))

(EXAMPLE (distance 42 11 82 3)(sqrt(+(sqr(line-length 42 82))(sqr(line-length 11 3)))))
(EXAMPLE (distance 16 91 72 56)(sqrt(+(sqr(line-length 16 72))(sqr(line-length 91 56)))))
(EXAMPLE (distance 0 0 4 3) 5)Collide takes in the distance between these objects and produces whether or not they are colliding based on if the range value is within the parameters of a specified amount. In the function, used as an example, this takes the coordinates and checks to see whether or not they are within 50 units of each other.

(define (distance px py cx cy)
  (sqrt(+(sqr(line-length px cx))(sqr(line-length py cy)))))


(EXAMPLE(collide 220 70 120 40)(<=(distance 220 120 70 40) 50))


(define (collide px py cx cy)(<=(distance px py cx cy)50))
```
## What does it do?

- This code is very intersting as each line correlates to the end result
  - Line-length takes in the coordinates of two objects in a straight line, and it outputs the difference using a conditional between two objects and outputs the distance between them specifically on one axis. This connects to distance, as it is needed to collect the data to help distance be completed and calculate the entire distance between two game objects based on their positions and the use of lines.
  - In addition, Distance calculates the coordinates of two game objects, and with this, uses pythagorean theorem to find the exact distance between the objects on both the x and y axis. Now this is correlation to the collide function as you use a boolean in order to figure out how to find if the game objects are colliding based on their distance.
  - Collide takes in the distance between these objects and produces whether or not they are colliding based on if the range value is within the parameters of a specified amount. In the function, used as an example, this takes the coordinates and checks to see whether or not they are within 50 units of each other.
