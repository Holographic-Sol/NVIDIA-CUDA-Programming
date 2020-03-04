For Developing, Compiling & Analyising.

GPU
1. Install All Required Software.
- CUDA cuda_10.2.89_441.22_win10
- vs_buildtools__768951616.1561046066

2. Environmental Variables:
needed for nvcc: C:\Program Files (x86)\Microsoft Visual Studio\2019\BuildTools\VC\Tools\MSVC\14.24.28314\bin\Hostx86\x64\
needed for nvprof: C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v10.2\extras\CUPTI\lib64

3. To Compile .cu code run: nvcc file.cu -o file

4. Profile: nvprof file.exe

CPU (Only neccessary if you wish to compare time taken for execution between cpu and gpu version of a program)
1. Install CygWin with gcc g++ compiler and nano

2. Environmental Variables:
needed for windows executables built using cygwin: C:\cygwin\bin

3. Use included PDF for help with gcc g++

4. Once compiled you can time execution with: Measure-Command {.\file.exe}