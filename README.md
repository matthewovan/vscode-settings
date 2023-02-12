# vscode-settings
Matt's custom vscode settings

## Who is this for?
For anyone coding c++, but specifically for the development environment at the University of Washington Bothell. However, with minor changes, 
the .devcontainer.json file can be modified to accomidate any docker environment.

## What's all of this?
This is a suite of files that make coding c++ in vscode a lot easier. It includes debugging, IntelliSense, Clang, and an automated docker container launcher.

## What does it all do?
The .devcontainer.jason launches any project in a docker container, whose image you specify. The rest enables clang-tidy, clang-format, IntelliSense, and debugging settings in VSCode.

## Useful commands

clang-format -i *{your filetype} // in-place formats all files with the designated filetype in your repo

clang-tidy *.cpp // this will check your code against the errors and warning enabled in the .clang-tidy file
                 // you can disable an error at the line it occurs using ` //NOLINT ` at the end of that line, 
                 // or ` // NOLINTBEGIN(check-name) ... // NOLINTEND(check-name) ` for a code block with a specified error (check-name) in mind.
                 
Pressing the F5 key // this starts the debugger

## Make sure you read through all the files before using the tools
Sometimes these files won't work for your sepcific development environment. You will likely have to change filenames, file paths, and output files to get this to work right.
I did my best to make it generic, but you might have to fix a few things to make it work smoothly for your projects.


