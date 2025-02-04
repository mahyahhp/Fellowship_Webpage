#### Compiling on Windows

To compile LISFLOOD-FP on Windows, [Microsoft Visual Studio](https://visualstudio.microsoft.com/) and [CMake](https://cmake.org/) are required. By default, CMake is installed as part of the **Desktop development with C++** workloads, in the process of installing Visual studio. 

To compile the LISFLOOD-FP code, either MSVC (the default C++ compiler of Visual Studio) or [Intel C++](https://software.intel.com/content/www/us/en/develop/tools/oneapi/components/dpc-compiler.html) compilers can be used. The compiling process is explained below for each of these compiler choices.


- **Using the MSVC compiler**

Launch Visual Studio and open `LISFLOOD-FP-trunk` as a local folder:

![image](/Figures/comp_win_1.png)
![image](/Figures/comp_win_2.png)

CMake build process will start automatically. After the build process is finished, from the *Configuration* drop-down list, choose `msvc-x64-Debug` or `msvc-x64-Release`:

![image](/Figures/comp_win_3.png)

From the *Build* menu click on *Rebuild All*:

![image](/Figures/comp_win_4.png)

After the compiling is finished the `lisflood.exe` executable file will be generated in `\LISFLOOD-FP-trunk\out\build\msvc-x64-Debug` or `\LISFLOOD-FP-trunk\out\build\msvc-x64-Release` sub-directories (depending on the configuration used above). 

- **Using Intel compiler**

In the `LISFLOOD-FP-trunk` directory, click on the `launch_vs2019_intel64.bat` script. This script sets the necessary environment variables for Visual Studio to locate the Intel compiler. At Visual Studio start window open `LISFLOOD-FP-trunk` as a local folder:

![image](/Figures/comp_win_1.png)
![image](/Figures/comp_win_2.png)

CMake build process will start automatically. After the build process is finished, from the *Configuration* drop-down list, choose `intel-x64-Debug` or `intel-x64-Release`:

![image](/Figures/comp_win_5.png)

From the *Build* menu click on *Rebuild All*:

![image](/Figures/comp_win_4.png)

After the compiling is finished the `lisflood.exe` executable file will be generated in `\LISFLOOD-FP-trunk\out\build\intel-x64-Debug` or `\LISFLOOD-FP-trunk\out\build\intel-x64-Release` sub-directories (depending on the configuration used above).

[back](/LISFLOOD8.0.md)
