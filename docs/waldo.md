#The Waldo Challenge

![waldo](waldo-images/maps_troy.jpg)

## Motivation

Any effective self driving system is going to need to be able to rapidly respond to it's environment. Often, the only cues it will get for its response is the visual around it (if a car swerves in front of you, or a pedestrian runs out, its unacceptable to wait until physical contact before hitting the breaks). Naturally then, its clear that computer vision is going to be a fundamental aspect of any self driving car. To kick off the first of our Challenges we shall present a problem in computer vision. 

## Challenge Description

Given a collection of images, some containing a stop sign, and others not, design a computer program to effectively determine which images do contain a stop sign and which don't. Your submission will be compared to other sibmissions based on accuracy and speed of execution.

## Format

The Programs will be submitted as a single directory containing 

```
install_dependencies.sh
compile.sh
run.sh
...
```

Your program needs to set itself up on a fresh install of Ubuntu 14.04. `install_dependencies.sh` should downloadany libraries and supporting files your program needs, and `compile.sh` will compile your program, if that's necessary. These will not be timed. The third must be set up so that it accepts a directory of png images.

```sh
run.sh path/to/directory/containing/images
```

This is the portion of your project that will be timed.

 The program must output JSON Array that pairs the filenames in the directory with a "1" (yes) /"0" (no) for whether a stop-sign is present or not present in the image respectively. A sample output  is shown below:

```sh
run.sh path/to/directory/containing/images 
[
    {	
    "filename": "college_ave_stopsighn.png",
        "stop_sign": "1"
    }, 
    {
    "filename": "hippopotamus.png",
    "stop_sign": "no"
    }
]
```

## Submission Instructions

Submissions will be accepted [here](https://github.com/DriveAI/challenges) as a pull request. To submit, we recommend that you fork the challenges repository. Add your project folder to the `submissions/waldo` folder. We'd also like you to contribute your test-dataset to our dataset to run against everyone in the competition. Drop all the images that you used into the `dataset/` folder. Over the course of the project these will quickly grow into a fairly large data set for high quality testing. Monitor your pull request, in case we have any trouble with your submission, this is how we'll contact you.

## Judging/Grading

Your submissions will be graded based on accuracy and speed, with a much higher weight on accuracy. We look forward to seeing everyone's submissions!
