# allMyOpenNNCode
I was able to create a visual studio project that uses openNN.

AFTER BUILDING THE OPENN USING CMAKE-GUI :
You will have additional directories.
My additional directory where I built is called build64.

Based on that, my settings to have everything working right in 
Visual Studio are:

(Project Settings is a window that comes up when you right-click the 
name of your project (hint: has a ++ icon next to it!) and then at the bottom
of the menu that pops up is 'Properties' and a drawing of a tool CLICK THAT THING).

Add to Project Settings -> 'VC++' -> Include Directories
C:\Users\Owner\Desktop\#project497\openNN\opennn_3.1\OpenNN;

Add to Project Settings -> 'VC++' -> 'Library Directories'
C:\Users\Owner\Desktop\#project497\openNN\opennn_3.1\OpenNN\build64\tinyxml2\Debug;
C:\Users\Owner\Desktop\#project497\openNN\opennn_3.1\OpenNN\build64\opennn\Debug;

Add to Project Settings -> C/C++ ->Additional Include Directories
C:\Users\Owner\Desktop\#project497\openNN\opennn_3.1\OpenNN\build64;
C:\Users\Owner\Desktop\#project497\openNN\opennn_3.1\OpenNN\build64\tinyxml2\Debug;
C:\Users\Owner\Desktop\#project497\openNN\opennn_3.1\OpenNN\build64\tinyxml2;
C:\Users\Owner\Desktop\#project497\openNN\opennn_3.1\OpenNN\build64\opennn;
C:\Users\Owner\Desktop\#project497\openNN\opennn_3.1\OpenNN\build64\tests;
C:\Users\Owner\Desktop\#project497\openNN\opennn_3.1\OpenNN\opennn;
C:\Users\Owner\Desktop\#project497\openNN\opennn_3.1\OpenNN\tinyxml2;

Add to Project Settings -> Linker -> Input
opennn.lib; 
tinyxml2.lib;

Also in my case, I built it for 64 bit (x64) so I go into Linker - all options,
scroll down and find 'Target Machine' - Set it to 64-bit (MACHINE-X64).
