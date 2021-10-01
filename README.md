# Yet Another Game Engine (YAGE)

A project written to better understand game engine design. Based on the [Magnum rendering engine](https://magnum.graphics/) and written in C++, using a GLFW backend. 

## To run
On windows, clone the repository with submodules as:
```bash
git clone --recurse-submodules https://github.com/vectorcrumb/YAGE.git
```
This will clone the corrade and magnum repos into the `external/` folder. Alongside these directories, GLFW is required. Download the Windows pre-compiled binaries from the [GLFW website](https://www.glfw.org/download.html). Place the `glfw-x.y.z.bin.WIN64/` folder in `./external/`. This project was developed with version 3.3.4 of GLFW. After this, normal build instruccions apply:
```bash
mkdir build
cd build
cmake ..
make
```
After this, run `YAGE.exe` in `build/Debug/bin/`.