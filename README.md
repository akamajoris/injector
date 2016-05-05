CLI DLL-Injector



About

Loader is an easy to use application that was designed to help you inject DLL libraries into running processes. The utility stops the process during injection. Loader will also provide you with detailed information if errors occur.


Complete control via the command line (Batch scriptable)
Target process is stopped during the injection
Output of all error messages
Map a PE file into the remote adress space of a process (without calling LoadLibrary).
Dump modules associated with the specified process id.
Inject x86 code into a x86 process (Use x86 loader)
Inject x64 code into a x64 process (Use x64 loader)
Tested on Windows XP/Vista/7.
Credits

typ312
ACB

Usage

injection via process id:

newloader --lib "C:\test.dll" --pid 0xD6C


injection via process name:

newloader --lib "C:\test.dll" --procname "TARGET.exe"


injection via window title:

newloader --lib "C:\test.dll" --wndtitle "Window Title"


injection via window class:

newloader --lib "C:\test.dll" --wndclass "ArenaNet_Dx_Window_Class"


injection on startup:

newloader --lib "C:\test.dll" --launch "C:\TARGET.exe" [--args "TARGET.exe param1 param2"] [--wii]


ejection via module address:

newloader --lib 0x74FE0000 --procname "TARGET.exe" --eject


ejection via module path:

newloader --lib "C:\test.dll" --procname "TARGET.exe" --eject


injection/ ejection with "SeDebugPrivilege":

newloader --lib "C:\test.dll" --procname "TARGET.exe" --dbgpriv


manual map:

newloader --lib "C:\test.dll" --procname "TARGET.exe" --mm


list all modules:

newloader --listmodules 0x123 > modules.txt




SOFTPEDIA "100% FREE" AWARD

http://www.softpedia.com/base_img/softpedia_free_award_f.gif' />

Softpedia guarantees that Loader 4.1 is 100% Free, which means it does not contain any form of malware, including but not limited to: spyware, viruses, trojans and backdoors.

This software product was tested thoroughly and was found absolutely clean; therefore, it can be installed with no concern by any computer user. However, it should be noted that this product will be retested periodically and the award may be withdrawn, so you should check back occasionally and pay attention to the date of testing shown above.

http://www.softpedia.com/get/Programming/Other-Programming-Files/Loader.shtml'>http://www.softpedia.com/get/Programming/Other-Programming-Files/Loader.shtml
