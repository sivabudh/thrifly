# thrifly
Playing around with Apache Thrift using Python, C#, and C++

What's Thrift? Read the layman's explanation here: https://www.quora.com/In-simple-terms-what-is-Thrift-software-framework-and-what-does-it-do

## Setting up your machine
1. Install chocolatey package manager. Follow the instructions from here: https://chocolatey.org/docs/installation
1. Then, if you are on Windows, do `choco install thrift`. If you are on a Mac, do: `brew install thrift`

## Setting up your project
1. Clone the source code
1. Go into the project's root directory

## Build instructions for each language

### C# / .NET
1. Visual Studio 2017
1. Windows 10 x64
1. Execute: `thrift -r --gen csharp tutorial.thrift`
1. Open Thriftsharp.sln
1. Use NuGet to install ApacheThrift v0.9.3
1. Build the solution
1. Run ThriftsharpServer first
1. Then, run ThriftsharpClient
1. Study the code and adapt to RING / POS
