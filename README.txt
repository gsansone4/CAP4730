A simple volumetric lighting simulation tool in OpenGL
Created by Jed Arnold and Gary Sansone for CAP4730 (UF, SP18)

Windows:
	- Clone/Download folder
	- Open Visual Studio solution and Run (Debug configuration)
	- Add the following:
		VC++ Include Directories: $(ProjectDir)external\glm-0.9.7.1;$(ProjectDir)external\glfw-3.1.2\include;$(ProjectDir)external\glew-1.13.0\include;$(IncludePath)
		VC++ Library Directories: $(ProjectDir)external\glm-0.9.7.1;$(ProjectDir)external\glfw-3.1.2\include;$(ProjectDir)external\glew-1.13.0\auto\lib;$(ProjectDir)external\glew-1.13.0\lib\Debug\Win32;$(LibraryPath)
		C/C++ Additional Includes: $(ProjectDir)external\glfw-3.1.2\include;$(ProjectDir)external\glm-0.9.7.1;$(ProjectDir)external\glew-1.13.0\include;$(ProjectDir);%(AdditionalIncludeDirectories)
		Linker Input Additional Dependencies: opengl32.lib;glu32.lib;external\glfw-3.1.2\src\Debug\glfw3.lib;external\Debug\GLEW_1130.lib;kernel32.lib;user32.lib;gdi32.lib;winspool.lib;shell32.lib;ole32.lib;oleaut32.lib;uuid.lib;comdlg32.lib;advapi32.lib;glew32d.lib;glew32sd.lib

Controls (need speeding up):
	- O: toggle occlusion or standard texture (not working yet)
	- R: toggle ray render

References:
	- www.opengl-tutorial.org
	- www.fabiensanglard.net/lightScattering/

Libraries:
	- GLM
	- GLEW
	- GLFW