##Precompiled DLL
After strugguling for a while to compile OpenCvSharp for MacOS I managed to build it using version 4.0.1 in Mojave.

- I installed OpenCv via homebrew (to satisfy the dependencies)
- Followed the instructions on how to build [here](https://github.com/shimat/opencvsharp/blob/master/Dockerfile)
- Referenced the library in my project

 ````
<PackageReference Include="OpenCvSharp4" Version="4.0.1.20190326"/>
<Reference Include="libOpenCvSharpExtern.dylib">
  <HintPath>libOpenCvSharpExtern.dylib</HintPath>
</Reference>
 ````
 
 I'll create a nuget package to make this easier, however for now you can download the compiled library if you don't want to build it yourself [here](libOpenCvSharpExtern.dylib)

##Useful links

[Build opencv and yolo with cuda support for MacOs](https://jacobysuh.com/blog/2018/computervision/)
