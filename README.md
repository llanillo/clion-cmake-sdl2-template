# Cmake and SDL2 Setup Tutorial

1. Downloaded the lastest [SDL Development Libraries](https://www.libsdl.org/download-2.0.php)
2. Downlad the [SDL2 Cmake Scripts](https://github.com/tcbrindle/sdl2-cmake-scripts)
3. Put FindSDL2.cmake into the "Modules" CMake subfolder.

If you use Clion the location is <CLion_istallation_path>\bin\cmake\win\share\cmake-(version)\Modules.

4. Download the CMakeLists.txt from this repository and replace all "NAME_PROJECT"
5. Put the SDL2.dll from the SDL Development folder into your cmake-build-debug folder
6. Modify the main.cpp to look like:

`int main (int argc, char* args[])`

**The exit code should be 0**
