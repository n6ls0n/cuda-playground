# README

A repository for the code from PMPP & PCCP and also a starter repo for making CUDA projects. It also contains the "cuda_samples" repo from NVIDIA.

As of 9/18/24, cuda_samples supports up to Toolkit 12.5 but the current SDK available for download is 12.6.1. See the instructions below to update the VS solutions to use the newer SDK

How to Update the CUDA Version in a Visual Studio Project:

1. Update CUDA Toolkit
Download and install the latest CUDA toolkit from the NVIDIA website.
Make sure to select the correct version for your system (Windows, x86 or x64).
2. Update Visual Studio Project Settings
Open your Visual Studio solution.
Right-click on the project that uses CUDA and select Properties.
In the Configuration Properties tree, navigate to C/C++ > General.
Update the CUDA Toolkit path to point to the newly installed CUDA toolkit directory (e.g., C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.2).
3. Update CUDA Build Customization
In the Solution Explorer, right-click on the project and select Build Customizations.
In the Build Customizations dialog, select the newly installed CUDA toolkit version (e.g., CUDA 11.2).
Click OK to apply the changes.
4. Update Project Dependencies (if necessary)
If your project uses any CUDA-dependent libraries (e.g., cuBLAS, cuDNN), you may need to update their versions to match the new CUDA toolkit version.
5. Rebuild and Verify
Rebuild your project to ensure that it compiles and links correctly with the updated CUDA toolkit.
