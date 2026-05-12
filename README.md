<img width="538" height="366" alt="image" src="https://github.com/user-attachments/assets/5baf8688-dc5c-4080-afad-1f536463c629" />
If you encounter the same problem Please allow this way to solve
first in source code dir where build a new "build" file and cd build


code(use Powershell):
cd D:\opencv_mingw_4.11
rmdir /s /q build
mkdir build
cd build


cmake .. -G "MinGW Makefiles" -DCMAKE_CXX_COMPILER=C:/Qt/Tools/mingw1310_64/bin/g++.exe -DCMAKE_C_COMPILER=C:/Qt/Tools/mingw1310_64/bin/gcc.exe -DCMAKE_RC_COMPILER="" -DOPENCV_DISABLE_CONFIGURATION_VERSIONING=ON -DCV_DISABLE_OPTIMIZATION=ON -DBUILD_SHARED_LIBS=OFF -DBUILD_PERF_TESTS=OFF -DBUILD_TESTS=OFF -DBUILD_EXAMPLES=OFF

mingw32-make -j4
