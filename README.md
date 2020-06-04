# rosinstalls
A common place to put rosinstall files, which are a nice way to organize names of related packages for installation together from source control.

# Usage
The easiest usage is to copy one of the rosinstall files to your new (empty) workspace so that you have something like
```
cd ~/new_test_ws/src/eva-maze.rosinstall
```
And then you can just run
```
wstool init . eva-maze.rosinstall
```
to clone all the repositories referenced in the .rosinstall file to your workspace. Proceed to build your workspace normally from the `~/new_test_ws/` folder.


# Further documentation
Excellent documentation on rosinstall files can be found at https://github.com/personalrobotics/pr-rosinstalls

A minimal example of rosinstall usage is available at https://github.com/travers-rhodes/rosinstalls

Additional documentation on `wstool` (the program that reads/interprets these rosinstall files) is available at http://wiki.ros.org/wstool
