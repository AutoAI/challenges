#The Waldo Challenge


## Motivation

Any effective self driving system is going to need to be able to rapidly respond to its environment. Often, the only cues it will get for its response is the visual around it (if a car swerves in front of you, or a pedestrian runs out, its unacceptable to wait until physical contact before hitting the breaks). Naturally then, its clear that Computer Vision is going to be a fundamental aspect of any self driving car. To kick off the first of our Challenges we shall present a problem in computer Vision. 
## Challenge Description

Given a collection of images, some containing a stop sign, and others not, design a computer program to effectively determine which images do contain a stop sign and which don't. 

## Format

The Programs will be submitted as a single file that accepts a single command line string, the path to a directory containing the  images. The program must print to console a JSON Array that pairs the filenames in the image with a "yes"/"no" for whether a stop-sign is present or not present in the image respectively. A sample submission is shown below:

    [
        {	
  	    "filename": "sid.png",
            "stop_sign": "yes"
        }, 
        {
	    "filename": "anotherfile.png",
	    "stop_sign": "no"
        }
    ]

## Submission Instructions

TBD, any submission must be paired with at least 15 images that do contain a stop-sign and 15 that do not into their respective folders. 

## Judging/Grading

Programs will be scored with the following metric \(  a^2 \) 
