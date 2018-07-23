# thrifly
Playing around with Apache Thrift using Python, C#, and C++

What's Thrift? Read the layman's explanation here: https://www.quora.com/In-simple-terms-what-is-Thrift-software-framework-and-what-does-it-do

## Setting up your machine
1. Install chocolatey package manager. Follow the instructions from here: https://chocolatey.org/docs/installation
1. Then, if you are on Windows, do `choco install thrift`. If you are on a Mac, do: `brew install thrift`

## Build instructions for each language
1. Clone the source code
1. Go into the project's root directory

### C# / .NET
1. Visual Studio 2017
1. Windows 10 x64
1. Execute: `thrift -r --gen csharp tutorial.thrift`
1. Open Thriftsharp.sln
1. Use NuGet to install ApacheThrift v0.9.3
1. Build the solution
1. Run ThriftsharpServer first
1. Then, run ThriftsharpClient
1. Study the code and adapt to RING + POS (.NET 3.5. C# 5) and PISS (.NET 4.5.1 C#7)

### Python
1. PostgreSQL 10 on macOS
1. Timescale (follow the instructions from here: http://docs.timescale.com/v0.10/getting-started/installation/mac/installation-homebrew)
1. Target OS is Windows 10 x64, but during development, use macOS first for speed and convenience
1. Use `pyenv` to install Python v3.7.0, and ensure you are using this version
1. `pip install -r requirements.txt`
1. Run server first: `python server.py`
1. Then, open another Terminal tab, run: `python client.py`
1. Study the code and adapt to PIDB project
