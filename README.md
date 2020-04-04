# vscodeOF
Using VSCode as a preprocessing and debug tool of OpenFOAM container

Steps to setup:
    1. Download/clone the folder from https://github.com/Microsoft/vscode-remote-try-cpp
    2. Launch VSCode and open the folder, reopen in container, click the Start Debugging button,
       make sure everything working as expected.
    3. Modify the Dockerfile
    4. Create codeSrc, codeBuild, ofCases 3 folders, delete main.cpp file
    5. cd to codeCases folder and run: cp -r $FOAM_TUTORIALS/incompressible/icoFoam/cavity/cavity .
    6. cd to codeSrc folder and run: cp -r $FOAM_SOLVERS/incompressible/icoFoam .
    7. modify the EXE in Make/files file: EXE = /workspaces/vscodeOF/codeBuild/icoFoam
    8. cd to icoFoam folder, run WM_COMPILE_OPTION=Debug and wmake. icoFoam should be built in codeBuild folder
    9. Modify tasks.json, launch.json (see the files for what have been changed)
    10. Click the Start Debugging button, the app be started and stop at the first line in the main function (see the screen shot)
    
