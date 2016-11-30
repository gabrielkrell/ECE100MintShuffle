# ECE100MintShuffle
Code for ECE 100 Competition 2; HandyBug that plays the "Mint Shuffle X" game, follows lines, and plays music.

This is a project for IIT's ECE 100: Intro to the Profession.  It won the course-wide Competition 1, accurately following a tape line faster than all other competitors, and came second place in the class's Competition 2.  Unfortunately, we didn't record the deciding match of Competition 2, where opposing strategies resulted in the winner being the robot that delayed longest before beginning their routine, but we did take a video of the robot's performance in the first competition.


Click here for video of the robot:

[![Competition 1 run](https://img.youtube.com/vi/UAIlM72JOs0/0.jpg)](https://www.youtube.com/watch?v=UAIlM72JOs0)


-----

The [Handy Board](https://en.wikipedia.org/wiki/Handy_Board) is a robot controller created at MIT for a 1996 robotics contest.  It's programmed in *Interactive C*, a limited subset of C which does not support:

 - Pointers
 - Booleans
 - Structs
 - Enums
 - Ordinary dynamic variable allocation. All local variables must be declared at the very beginning of a function (e.g. no initialization in `for` loops).
 
Despite its limitations, IC comes with libraries for controlling robot peripherals and task scheduling, so it's possible to implement reasonably advanced things without enough time.
 
-----
 
Load mshuffle.lis to load all the component files at once.  `main()` is in `mshuffle.ic`, motor control functions are in `mshuffle_motors.ic`, sensor stuff and the configuration routines that involve them are in `mshuffle_sensors.ic`.
