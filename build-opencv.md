
# Windows build

## get source code

download opencv package from this link
https://sourceforge.net/projects/opencvlibrary/files/opencv-win/3.4.1/opencv-3.4.1-vc14_vc15.exe/download

install the package to OPENCV_DIR, the source code is extracted in this path:
OPENCV_DIR\opencv\sources

## generate Visual Studio project with cmake

create a **build** folders for 32bit and 64bit build respectively

OPENCV_DIR\opencv\build32
```dos
cd build32
cmake ..\sources
```

OPENCV_DIR\opencv\build64
```dos
cd build64
cmake -DCMAKE_GENERATOR_PLATFORM=x64 ..\sources
```

## build project

open the **OpenCV.sln** with Visual Studio in build32 or build64 folder and run build solution in VS

# Ubuntu 16.04 build
