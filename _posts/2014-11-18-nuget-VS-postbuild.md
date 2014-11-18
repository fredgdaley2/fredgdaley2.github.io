---
published: true
---

## Nuget post build event command for Visual Studio

To have Visual Studio automatically build a Nuget package when building add the following to the post event.

Copy and paste command:
     
     nuget pack "$(ProjectPath)" -IncludeReferencedProjects
     
     
The Nuget package will be put in the bin\<current build type> folder 
Bin\Degug or Bin\Release which ever is chosen not both at the same time.