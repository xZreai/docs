# Development Environment

## Required Software, Tools and libraries
- git / github
- Docker
- IDE (Visual Studio Code, Jetbrains, etc.)

## Getting the source code

!!! error "TEMP"

Before you can load the project to test in your simulator, you first need to ensure you've created a fork of the [A32NX project on GitHub](https://github.com/flybywiresim/a32nx){target=new} and have cloned this in your code editor/IDE.
We recommend when making changes on your fork, you create a new branch, titled with the change you're looking to make or something similar.
Make sure you have also run the setup and build scripts shown below and explained in detail on [GitHub Contributing.md](https://github.com/flybywiresim/a32nx/blob/master/.github/Contributing.md){target=new}.

```
git clone https://github.com/flybywiresim/a32nx.git
cd a32nx
.\scripts\dev-env\run.cmd ./scripts/setup.sh
.\scripts\dev-env\run.cmd ./scripts/build.sh
```

## Compiling the source

## Linking Dev folder to Community folder

Once you have the A32NX built, you'll need to link your newly compiled A32NX to your community folder to enable you to quickly update the flyPad with new changes made to your local branch without copying everything over manually again and reloading MSFS.
This is commonly referred to as a 'Symlink'.

To create your Symlink, open your command terminal and run the below command, substituting the correct file paths with your community folder, and the 'flybywire-aircraft-a320' folder from your new project.

!!! warning "Important step!"
    Make sure you remove any existing copy of the aircraft from your community folder before doing this.

```
mklink /J [MSFS Community folder/flybywire-aircraft-a320-neo] [Project folder path]
```
Example:
```
mklink /J C:\Users\USERNAME\AppData\Local\Packages\Microsoft.FlightSimulator_8wekyb3d8bbwe\Community\flybywire-aircraft-a320-neo C:\Users\USERNAME\IdeaProjects\a32nx\flybywire-aircraft-a320-neo
```

If this works, you'll receive the response:

"Junction created for \[Community folder] \[Project Folder]" from the terminal.

Now you've compiled and symlinked your Github fork to your community folder, you should be able to load into the aircraft as normal. Open MSFS and check everything is working with your compiled branch before progressing.

## Hello World Example

## Quick reloading of avionics displays

## Tips & Tricks

## Troubleshooting


