---
title: "moving files around and knowing what is already there"
output: html_document
date: "2024-03-26"
---


:::::: questions
 - question 1
 - question 2
::::::

:::::: objectives
 - objective 1
 - objective 2
::::::

## moving files around

Rclone is most frequently used to move files, individually or as a group from one place to another.


## The syntax for the places, to or from is:

**source:folder     destination:folder**  

#### or

**local/path  remote/path**   

## Examples:

#### My home backup of local to an external drive (windows using linux subsystem)
rclone copy /mnt/d/work-related /mnt/f/work-related-backup


## Note: Different operating systems have __slightly__ different syntax 

Windows syntax:   rclone ls C:\Users\jjamison\rclone
Linux syntax:  rclone ls /mnt/c/Users/jjamison/rclone


## valid remote names  
[https://rclone.org/docs/#valid-remote-names](https://rclone.org/docs/#valid-remote-names)

## Moving, syncing and knowing what is already there  
rclone **ls** remote:path # **lists contents of a remote**
rclone **copy** /local/path remote:path # **copies&& /local/path to the remote
rclone **sync** --interactive /local/path remote:path # **syncs** /local/path to the remote

## Reference:
[https://rclone.org/docs/#subcommands](https://rclone.org/docs/#subcommands)

Windows [https://rclone.org/docs/#windows](https://rclone.org/docs/#windows)   

Linux  [https://rclone.org/docs/#linux-osx](https://rclone.org/docs/#linux-osx)

:::::: keypoints
 - keypoint 1
 - keypoint 2
::::::
