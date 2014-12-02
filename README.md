# Aim/Goal

- The aim of this project is to develop simple tools and procedures to help developers keep their projects and code in conformity with a set of predefined standards.

- Create tools and procedures to easily check existing (legacy) projects against a set of predefined standards.

- Create tools and procedures to help developers create new projects that conform with predefined standards.


# Why?

- The code we write and the projects we create should be regarded as highly valuable. If you  see your project as important you will want to make sure it is properly maintained.

Making it **easy** to maintain is really what this project is all about.


# Introduction

One would think that the tooling to check a project "integrity" was well established by now in the .NET eco system.

We have not found this to be the case.
We are creating this project to try and resolve this issue or at leas give some pointers on how this can be achieved.

- Everything needs to be automated.
	- From creating a project with "batteries included" and the correct folder structure
	- To building **and deploying** the libraries.
- Everything should be as simple and quick as possible.


# Creating a project with "batteries included"

Please see: https://github.com/Orcomp/SolutionGenerator

- Stylecop settings
- Resharper settings
- Build and deployment scripts
- gitignore
- gitattributes
- Correct project structure

# Project structure


# Coding Standards

We follow 99.9% of the standards outline here: https://csharpguidelines.codeplex.com/

The only differences are:

- Use underscores for private fields ```(private string _myString;)```
- Remove ```This.``` keywords
- Use regions as little as possible. ([I Hate #Regions](http://visualstudiogallery.msdn.microsoft.com/0ca60d35-1e02-43b7-bf59-ac7deb9afbca) VS extension.)

# Repository

- Project guidelines (coding standards and project structure) are found in the "doc" folder.)
- Summary of project guidelines: http://www.geertvanhorrik.com/2012/04/04/setting-output-directories-of-projects/
- Stylecop settings we follow
- gitignore file

You must have [Stylecop](https://stylecop.codeplex.com/) installed. If not install it and restart your computer.

# Links:

- General standards link: http://stackoverflow.com/questions/14967/are-there-any-suggestions-for-developing-a-c-sharp-coding-standards-best-pract
- Sharing Resharper settings: http://blogs.jetbrains.com/dotnet/2011/12/resharper61-settings-dropbox-and-company-wide/
- http://jkanczler.wordpress.com/2013/09/27/share-style-cop-compatible-resharper-settings-between-different-machines/
- [Developer's Seven deadly sins](http://docs.codehaus.org/display/SONAR/Developers%27+Seven+Deadly+Sins)
- View Assembly Reference conflicts: http://mikehadlow.blogspot.co.uk/2013/10/asmspy-coloured-output.html
- Approval Tests: http://approvaltests.sourceforge.net/

# Recommended software

- [Stylecop](https://stylecop.codeplex.com/)
- [Resharper](http://www.jetbrains.com/resharper/)
- [FAKE F# Make](http://fsharp.github.io/FAKE/)
	- It is worth looking at existing open source projects that use FAKE to learn from their scripts.
- [SonarQube](http://www.sonarqube.org/)
	- For C#. http://docs.codehaus.org/display/SONAR/C%23+Ecosystem
	- https://github.com/SonarCommunity/sonar-dotnet
- [SonarQube Resharper plugin](https://github.com/SonarCommunity/sonar-dotnet-resharper)
- [Resharper InspectCode](http://confluence.jetbrains.com/display/NETCOM/Introducing+InspectCode)
	- with [viewer](http://weblogs.asp.net/fbouma/jetbrains-inspectcode-result-file-viewer)
- [Resharper dupFinder](http://confluence.jetbrains.com/display/NETCOM/Introducing+ReSharper+Command+Line+Tools)
