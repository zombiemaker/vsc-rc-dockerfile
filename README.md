# Template for Visual Studio Code Development Container Project

## What Is This?

This is simply a template for creating projects in Visual Studio Code where you want to create your programs inside a Linux container. 

## Why Use This?

When working on different types of software projects you may find that you use different combination of software programs (i.e. tools) to organize, edit, configure, build, test, package, distribute, etc..  

For example, if you are working on a software component built using Java 11 and Quarkus framework / runtime environment, you will have a set of supporting program libraries and tools that are optimized for producing that type of software component.

If you then have a project to work on a software component that uses APIs and program libraries that run in Node.js 14, that would be a different set of tools.

Likewise for a WebAssembly software component using AssemblyScript, C# and Blazor, C/C++ and enscripten, etc.

Likewise for a Python software component....

etc.

You don't want to pollute your main workstation environment with all of these different software components and potentially their different versions.

One way to do this is to use development containers that have the software components you need JUST FOR THE SPECIFIC TYPE of software component you are building. 

## Prerequisites

* Microsoft Windows Software
  * Microsoft Windows Subsystem for Linux 2
  * Docker Desktop for Windows using WSL2 engine configured for Linux containers not Windows containers
  * Linux WSL2 distro
  * git (for Windows)
  * Visual Studio Code
  * Visual Studio Code Extensions
    * Remote Development pack (inlcudes Remote - WSL, Remote - Containers, etc)
    
* Linux software for WSL2 distro
  * Docker Community Edition
  * git

## How To Use This

* Open this project folder from within a Linux environment (e.g, WSL instance) that has Docker engine installed
* Review the [README.md file](.devcontainer/README.md)
* Configure the .devcontainer/devcontainer.json file to your needs
* Reopen project folder in a container