# vscodeOF
Using VSCode as a preprocessing and debug tool of OpenFOAM container

Prerequirements:
   1. Docker is installed.
   2. VSCode with remote-container extension is installed.

How to start:
   1. Download or clone the vscodeOF folder from https://github.com/yyhx78/vscodeOF
   2. Launch VSCode and open the vscodeOF folder, click the "Editing .." button at the bottom left corner and select Remote-Containers: Reopen in container. The container will be built.
   3. cd to the codeSrc/icoFoam folder and run run WM_COMPILE_OPTION=Debug and wmake.
   4. Click the Run button in the left toolbar, then click Start Debugging at the top, icoFoam should be launched and stop at the begining of the main funciton.

See https://yyhx78.blogspot.com/2020/04/using-vscode-as-preprocessing-and-debug.html for the detail steps to generate the files and setup the environment.
