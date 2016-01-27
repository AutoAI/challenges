#The Waldo Challenge


## Motivation

Any effective self driving system is going to need to be able to rapidly respond to its environment. Often, the only cues it will get for its response is the visual around it (if a car swerves in front of you, or a pedestrian runs out, its unacceptable to wait until physical contact before hitting the breaks). Naturally then, its clear that Computer Vision is going to be a fundamental aspect of any self driving car. To kick off the first of our Challenges we shall present a problem in computer Vision. 
## Challenge Description

Given a collection of images, some containing a stop sign, and others not, design a computer program to effectively determine which images do contain a stop sign and which don't. 

## Format

The Programs will be submitted as a single directory containing 

    install_dependencies.sh
    compile.sh
    run.sh
    ... (other files)i
the first two bash files will be used to set up your program. The third must be set up so that it accepts a single command line string,the path to a directory containing the  images.

    ~ run.sh path/to/directory/containing/images

 The program must print to console a JSON Array that pairs the filenames in the directory with a "yes"/"no" for whether a stop-sign is present or not present in the image respectively. A sample output  is shown below:

    ~ run.sh path/to/directory/containing/images [
        {	
  	    "filename": "sid.png",
            "stop_sign": "yes"
        }, 
        {
	    "filename": "anotherfile.png",
	    "stop_sign": "no"
        }
    ]

Programs will be graded on a machine running UBUNTU 14.04. Please make sure your submissions are compatible with that. 

## Submission Instructions

We will be using github to organize the challenge. Submissions need to be made in the form of pull requests. Within https://github.com/DriveAI/challenges.git you should find a folder "Submissions", inside of which will be a folder "Waldo". A pull request must be made to submit your project folder into this folder. Furthermore there will be a folder in "Waldo" labelled "datasets" inside of which will be a folder labelled "Yes" and another labelled "No". These folders will contain images with stop-signs and without stop-signs respectively. With each Submission you must also submit 15 images to each folder (you can divide it up amongst group members). Over the course of the project these will quickly grow into a fairly large data set for high quality testing.


## Judging/Grading

Programs will be scored with the following metric TBD
