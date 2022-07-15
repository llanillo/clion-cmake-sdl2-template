# Clion and SDL2 Setup Tutorial

It's been so hard to find a decent guide about how to set up Clion and SDL2 so I made one for my future self and for some random person on internet who find this. I hope it helps you.

We are going to use the bunblded MinGw 64 bits version that comes with Clion, if you use 32 bits version you should replace the CMakeList file with the proper directory path.

1. Download the lastest [SDL Development Libraries (MinGW version)](https://www.libsdl.org/download-2.0.php)
2. Downlad the [SDL2 Cmake Scripts](https://github.com/tcbrindle/sdl2-cmake-scripts)
3. Create a new project with Clion
4. Create a cmake/modules directory in your project root and unzip all cmake scripts (downloaded from step 2) there.
5. Unzip the SDL Development libraries (downloaded from step 1) in your project root, rename the folder to 'SDL2'
6. Mark the SDL2 folder as excluded in Clion
7. Download the CMakeLists.txt from this repository, replace all the "PROJECT_NAME" with your project's name and add the file to your project root (replacing the create automatically)
8. Put the SDL2.dll from the SDL2 folder into your cmake-build-debug folder:
- For 64 bits version it's located in x86_64-w65-mingw32/bin/SDL2.dll
- For 32 bits version it's located in i686-w64-mingw32/bin/SDL2.dll

9. Modify the main.cpp to look like:

`int main (int argc, char* args[])`

If your exit code is 0 and Clion detects your SDL2 headers then you are good to go.

### Important

* MingGw should be the default toolchains for Clion
* Add the SDL2 and cmake folder to your gitignore


### The project tree should look like this
<p align="center">
  <img src="Example.png" />
</p>
