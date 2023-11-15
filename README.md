# Creating your first DOTNET project

At the bottom of the screen you will find the terminal.

```
@YourAccountName -> /workspaces/CSharp_FirstProject (main) $
```

> This is your command line. You can use this to interact with your computer, run programs, and navigate your files. You type in commands and keywords to perform action.

## Step 1 - Creating a New Console Project

1. Click on the terminal window. You should see a little square appear. You can now type on the keyboard.

Type in
```terminal
    dotnet new console --use-program-main
```
Example: `YourAccountName -> /workspaces/CSharp_FirstProject (main) $ dotnet new console --use-program-main`

2. Press **enter**.

***Result***. 
In the explorer to the right, you should see two new files appear.

* CSharp_FirstProject`.csproj`
* Program`.cs`

**CSharp_FirstProject`.csproj`** is file that contains a list of all the files required for our new C# project.  
**Program`.cs`** is our CSharp file. This file is where we will write our code. 

---

## Step 2 - Opening Your Project

There are 2 ways of opening our `Program.cs` file. 
    1. Click on the `Program.cs` file
    2. Type `Program.cs` into our terminal.

We're going to do the second.

1. Click on the terminal, and type

```
dir
```

***Result***
```
@YourProjectName ➜ /workspaces/CSharp_FirstProject (DevelopmentBranch) $ dir
CSharp_FirstProject.csproj  Program.cs  README.md  obj
```

> `dir` is a terminal command that displays all of the file in our folder. You'll notice the files are the same as in the explorer to the left. They are showing us the same thing, the current files in the folder.

***The next step will open up a new window here, you can get back to this file by clicking on the `README.md` tab on the top.***

2. Type `code Program.cs` into the terminal

Ex. `@YourProjectName ➜ /workspaces/CSharp_FirstProject (DevelopmentBranch) $ code Program.cs`

***Result***

`Program.cs`
```csharp
    namespace CSharp_FirstProject;

    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello, World!");
        }
    }

```

Your program file will open in visual studio code!

> `code <filename>` is a command that will open a file in Visual Studio Code. The syntax is the word code, followed by the filename, including the extension ( everything following the period ). .cs is the file extension for C# files
> - Good (with file extension) : `code Program.cs`
> - Bad ( no file extension ): `code Program`

## Step 3 - Running your code



