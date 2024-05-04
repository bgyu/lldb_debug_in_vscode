# Example to compile and debug C++ (with lldb) under Linux via ssh in VS Code (Windows)

This is an example to show you how to use VS Code under Windows,
and connect to remote Linux system via ssh,
and compile and debug C++ code with cmake and lldb.

## Prerequisite
* Need to install extension codelldb
  Reference: https://github.com/vadimcn/codelldb/blob/v1.10.0/MANUAL.md
* C/C++ (Microsft)
* C/C++ Extension Pack (Microsoft)
* CMake
* CMake Tools
* Remote SSH
* Remote Explorer

## Tasks to compile and install the binaries
All tasks are defined in .vscode/tasks.json. This json file is used to compile the code.

Ctrl + Shift + B and select "Debug Build" from the list.
It will start the "clean", then "Debug Config" task, and finally "Debug Build" task to build the final code.

To debug the code, you have to install the binary to a folder.
Ctrl + Shift + P and select "Tasks: Run Task", then select "Debug Install",
it will install the final binary "Hello" to `{workspaceFolder}/build/debug/bin`.

## Debug
launch.json is used for launch debugger.
Just set a breakpoint in the source code and press F5.
