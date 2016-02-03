## Cannon Fire ##

### DEPENDENCIES ###
----------------------------------------------------------------
Linux/Windows/ Mac OSX - Dependencies: (Recommended)
 GLFW
 GLAD
 GLM

Linux - Dependencies: (alternative)
 FreeGLUT
 GLEW
 GLM

----------------------------------------------------------------
### INSTALLATION ###
----------------------------------------------------------------
#### GLFW: ####
 - Install CMake  
 - Obtain & Extract the GLFW source code from  
   https://github.com/glfw/glfw/archive/master.zip  
 - Compile with below commands  
   $ cd glfw-master   
   $ mkdir build  
   $ cd build  
   $ cmake -DBUILD_SHARED_LIBS=ON ..  
   $ make && sudo make install  

#### GLAD: ####
 - Go to http://glad.dav1d.de  
 - Language: C/C++  
   Specification: OpenGL  
   gl: Version 4.5  
   gles1: Version 1.0  
   gles2: Version 3.2  
   Profile: Core  
   Select 'Add All' under extensions and click Generate.  
 - Download the zip file generated.  
 - Copy contents of include/ folder in the downloaded directory  
   to /usr/local/include/  
 - src/glad.c should be always compiled along with your OpenGL   
   code  

#### GLM: ####
 - Download the zip file from   
   ```https://github.com/g-truc/glm/releases/tag/0.9.7.2```  
 - Unzip it and copy the folder glm/glm/ to /usr/local/include  

  Ubuntu users can also install these libraries using apt-get.  

-----------------------------------------------------------------
### Execution ###

#### To execute the code run the makefile ####  
 $> make  
 $> ./sample2D  

```If the makefile gives errors or doesn't executes the code, execute using the following command.```  
 $> g++ -o sample2D Sample_GL3_2D.cpp glad.c -lglfw3 -lGL -lm -lXrandr -lXi -lX11 -lXxf86vm -lpthread -lGLU -ldl  
 $> ./sample2D  

-----------------------------------------------------------------

## Controls ##

1. Press key 'A' or 'a' for rotating the cannon upwards.
2. Press key 'B' or 'b' for rotating the cannon downwards.
3. Press key 'F' or 'f' to increase the speed.
4. Press key 'S' or 's' to decrease the speed.
5. Press SPACE to shoot.
6. Press UP arrow to zoom in and DOWN arrow to zoom out.
7. Press LEFT arrow to pan left and RIGHT arrow to pan right.

--------------------------------------------------------------------

## Game ##

The game objective is to hit the object on the wall.
Shoot a ball using the cannon to hit the object.
You can rotate the cannon or increase the speed of projection using the controls.

--------------------------------------------------------------------
