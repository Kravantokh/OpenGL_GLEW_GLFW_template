# OpenGL_template #

Basic OpenGL project template for c++ with CMake, glfw and gl3w meant to work out of the box on Windows and Linux and eliminate as much frustration as possible in the setup phase of any OpenGL project.

## Cloning ##
You should clone the repository with\
`git clone --recursive https://github.com/Kravantokh/OpenGL_GLEW_GLFW_template/`\
\
If you have already cloned it without `--recursive` you may download the submodules with\
`git submodule init` and then\
`git submodule update`.

## Current code ##

The file `src/main.cpp` contains a basic example code which creates an openGL context and opens it in a window with the help of glfw.

## Prerequisites ##
* CMake (obviously)
* GNU GCC: g++ (mingw on windows)
* ninja
* glu\*
* Python (3 or 2 should both work)


\*Linux-only dependency - may be installed with the package manager, in may case the command was `sudo pacman -S glu`
This package may have a different name under other distros.

## Build process ##
* Windows: run `build.bat`
* Linux: run `build.sh`

On linux don't forget to run `chmod +x build.sh`.

Until now the build process has been succesfully tested on Arch Linux, Kubuntu 20.10 and Windows 10 with the mentioned build tools.

## Errors you may meet ##

`XInput headers not found; install libxi development package` - Installing the package `xorg-dev` may help on Ubuntu/Kubuntu.

