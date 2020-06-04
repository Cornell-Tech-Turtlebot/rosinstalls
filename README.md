# rosinstalls
A common place to put rosinstall files, which are a nice way to organize names of related packages for installation together from source control.

# Quick Start
## To create:
1. wstool init
2. wstool scrape

## To check:
```
wstool status
wstool info
```

## To specify branch inside a .rosinstall file:

version: <branch name>


## To run:
1. Pull file and copy to, for example `~/new_test_ws/src/eva-maze.rosinstall`
2. wstool init . <rosinstall filename>
This will clone all the repositories referenced in the .rosinstall file to your workspace. Proceed to build your workspace normally from the `~/new_test_ws/` folder.


# Further documentation
Excellent documentation on rosinstall files can be found at https://github.com/personalrobotics/pr-rosinstalls

A minimal example of rosinstall usage is available at https://github.com/travers-rhodes/rosinstalls

Additional documentation on `wstool` (the program that reads/interprets these rosinstall files) is available at http://wiki.ros.org/wstool
