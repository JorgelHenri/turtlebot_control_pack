THIS CODE IS A MODIFICATION OF OCLPIXELGAMEENGINE - PATH FINDING WAVE PROPAGATION

OBJECTIVE

   GIVE A OCCUPANCY MATRIZ TO MADE A MAP, WITH A PATH DEFINE BY WAVE PROPAGATION
   
TIP TO BUILD THE MAP

1 - USE A BMP OR PNG IMAGE OF YOUR MAP, THAT BLACK IS WALL AND WHITE IS GROUND

2 - IN MATLAB USE THIS SINTAX

   - image = imread('mapaexemplo.bmp');
   
   - grayimage = rgb2gray(image);
   
   - bwimage = grayimage < 0.5;
   
   - grid = robotics.BinaryOccupancyGrid(bwimage, ​res​ );
   
      - RES IS PIXEL PER METER
   
   - show(grid) 
   
     - THIS IS YOUR MAP IN A GRID
   
     - TO AJUST THE ROBOT SIZE, INFLAT YOUR MAP WITH THIS SINTAX
   
   - robotRadius = 0.1;
   
     - 0.1 IS THE RADIUS OF THE ROBOT (IN THE SAME RES OF THE MAP)
   
   - mapInflated = copy(grid);
   
   - inflate(mapInflated,robotRadius);
   
   - show(mapInflated)
   
     - THIS IS YOUR INFLATED MAP, THAT IS THE MAP FOR THE ALGORITM READ TO CALCULATE A RIGHT PATH
     
     - TO EXPORT THIS MAP IN A MATRIZ FOR USE THE SINTAX
   
   - mat = occupancyMatrix(map)
   
     - IN THE MAP FILE YOU WILL HAVE YOUR MATRIZ, USE CTRL A TO SELECT ALL AND CTRL V TO PASTE THIS IN A TXT FILE, THE MATRIZ WILL BE TRUE AND FALSE VALUE, CHANGE THIS FOR 1 AND 0, ALSO CHANGE ALL THE DOUBLE SPACES TO SINGLE SPACE
     
SETTING THE CPP FILE

1 - TAKE A MATRIZ OF A IMAGE, THE MATRIZ HAS TO BE 1 FOR WALL AND 0 FOR GROUND

2 - PUT THIS MATRIZ IN A TXT FILE (THE MATRIX MUST CONTENT JUST "SPACE", 0 AND 1)

3 - SET THE FILE NAME IN READM MATRIX CLASS

4 - SET YOUR START AND END POINT

5 - IN THE MAIN FUNCTION USE THE MATRIZ SIZE IN THE DEMO.CONSTRUCT (SIZE_X, SIZE_Y, PIXELRATE_X, PIXELRATE_Y)       [RECOMMENDED USE PIXEL RATE 1 ,1]


# olcPixelGameEngine
The official distribution of olcPixelGameEngine, a tool used in javidx9's YouTube videos and projects.

**You only need the one file - olcPixelGameEngine.h - included in your project!**

Provides a fast, richly featured, cross platform pixel drawing and user interface framework for
 * The development of games
 * Visualisation of algorithms
 * Prototyping and experimentation
 * Education

olcPixelGameEngine is easily extended! for example:
 * 2D Affine transforms
 * 3D Software renderer
 * Controller input
 * Sound
 * Hardware interfaces
 
olcPixelGameEngine is easy to port! Runs on:
 * Windows (all)
 * Linux / Raspberry Pi / ChromeOS
 * MacOS (coming soon to official, but already available in "Contributors")
 * PSP & Switch (Not supported by OneLoneCoder)
 
olcPixelGameEngine has been reimplemented in other languages!
 * C#
 * Rust
 * Lua
 * Java
  
olcPixelGameEngine is actively maintained and developed!

olcPixelGameEngine is used by 100s, if not 1000s of programmers at all levels of ability!


# Documentation
Please see https://github.com/OneLoneCoder/olcPixelGameEngine/wiki

# License (OLC-3)

Copyright 2018, 2019, 2020 OneLoneCoder.com

Redistribution and use in source and binary forms, with or without 
modification, are permitted provided that the following conditions 
are met:

1. Redistributions or derivations of source code must retain the above 
   copyright notice, this list of conditions and the following disclaimer.

2. Redistributions or derivative works in binary form must reproduce 
   the above copyright notice. This list of conditions and the following 
   disclaimer must be reproduced in the documentation and/or other 
   materials provided with the distribution.

3. Neither the name of the copyright holder nor the names of its 
   contributors may be used to endorse or promote products derived 
   from this software without specific prior written permission.
    
THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS 
"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT 
LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR 
A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT 
HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, 
SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT 
LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, 
DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY 
THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT 
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
