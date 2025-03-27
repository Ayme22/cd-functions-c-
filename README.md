# cd-functions-c++
Directory Navigation Tool (C++)
This tool allows you to navigate through directories in a Windows environment using simple commands, such as cd <directory_path>, .. to move back one directory, and quit to exit the program.

Features
Display the current working directory.

Change to a specified directory using the cd <directory_path> command.

Move up one directory using the .. command.

Exit the program using the quit command.

Prerequisites
A Windows operating system (the program uses SetCurrentDirectoryW which is Windows-specific).

A C++ compiler (such as Microsoft Visual Studio, MinGW, etc.).

C++17 or later for std::filesystem.

How to Compile
Using Microsoft Visual Studio:
Open Microsoft Visual Studio.

Create a new C++ console project.

Copy the provided code into your project's main source file (e.g., main.cpp).

Ensure that your project is set to use C++17 or later:

Right-click on your project in the Solution Explorer.

Select Properties.

Under Configuration Properties, go to C/C++ > Language.

Set C++ Language Standard to ISO C++17 or later.

Build and run the project (press Ctrl + F5).

Using MinGW or another GCC-compatible compiler:
Save the code in a file, e.g., directory_navigation.cpp.

Open a command prompt or terminal.

Navigate to the directory where the file is located.

Run the following command to compile the program:

bash
Copy
g++ -std=c++17 directory_navigation.cpp -o directory_navigation
After compilation, run the program:

bash
Copy
directory_navigation.exe
Usage
When you run the program, it will display the current directory and prompt you for a command.

Commands:
cd <directory_path>: Change to the specified directory.

Example: cd C:\Users\Username\Documents

..: Move up one directory.

quit: Exit the program.
