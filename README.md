# Creating your first DOTNET project

At the bottom of this screen you will find the terminal.

```
@YourAccountName -> /workspaces/CSharp_FirstProject (main) $
```

> This is the terminal ( aka command line ). You can use this to interact with your computer, run programs, and navigate your files. You type in commands and keywords to perform action.

## Step 1 - Creating a New Console Project

1. Click on the terminal window. You should see a little square appear. You can now type on the keyboard.

Type in
```terminal
    dotnet new console --use-program-main
```
Example: **`YourAccountName -> /workspaces/CSharp_FirstProject (main) $ dotnet new console --use-program-main`**

2. Press **enter**.

***Result***. 
In the explorer to the right, you should see two new files appear.

* CSharp_FirstProject`.csproj`
* Program`.cs`

**CSharp_FirstProject`.csproj`** is file that contains a list of all the files required for our new C# project.  
**Program`.cs`** is our CSharp file. This file is where we will write our code. 

> **Breakdown**
> - **`dotnet new console --use-program-main`**
> - **`dotnet`** - dotnet is the C# code framework. It lets us create C# projects
> - **`new console`** - this tells dotnet to create a new C# Console project in the current folder
> - **`--use-program-main`** - this adds an important template to our project

---

## Step 2 - Opening Your Project

There are 2 ways of opening our **`Program.cs`** file. 
1. Click on the **`Program.cs`** file
2. Type **`Program.cs`** into our terminal.

We're going to do the second.

1. Click on the terminal, and type

```
ls
```

***Result***
```
@YourProjectName ➜ /workspaces/CSharp_FirstProject (DevelopmentBranch) $ ls
CSharp_FirstProject.csproj  Program.cs  README.md  obj
```
> **`ls`** is a terminal command for "list." It displays all the files in our current folder. Notice that the files are identical to the Explorer to the left. They are showing us the same thing: the current files in the folder.

***The next step will open up a new window here; you can return to this file by clicking on the **`README.md`** tab on the top.***

2. Type **`code Program.cs`** into the terminal

Ex. **`@YourProjectName ➜ /workspaces/CSharp_FirstProject (DevelopmentBranch) $ code Program.cs`**

***Result***

**`Program.cs`**
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

> **`code <filename>`** is a command that will open a file in Visual Studio Code. The syntax is the word code, followed by the filename, including the extension ( everything following the period ). .cs is the file extension for C# files
> - Good (with file extension) : **`code Program.cs`**
> - Bad ( no file extension ): **`code Program`**

## Step 3 - Running your code

1. Now that we have our code lets run it. We will learn 2 new commands.
- **`dotnet build`**
- **`dotnet run`**

The **`dotnet build`** command **Compiles** our code. That means it converts our C# into code the computer can understand and run.

**`dotnet run`** will run our code after **`dotnet build`** is done.

**Type**
```
dotnet build
```

```csharp
    Build succeeded.
        0 Warning(s)
        0 Error(s)
```

If your code is working, you should see a message that says **"Build Succeeded"**. If it says Build Failed, or you have more than 0 errors, you need to fix errors in your code before it can build.

2. **Type `dotnet run`**

***Result***.  
**`Terminal`**
> Ex: **`Hello, World!`**

And it runs!

If your **`dotnet build`** was successful, then when you run **`dotnet run`** your code from our **`Program.cs`** file will run.

Let's practice 1 more time.

---
## Practice

In your csharp file, on line 7, you will see a line that says.

```csharp
    Console.WriteLine("Hello, World!");
```
***Replace the word World, with your name***

> Ex: **`Console.WriteLine("Hello, Will!");`**

**Save your code**

Then type
1. **`dotnet build`**
    - If failed double check your code for errors
2. **`dotnet run`**

***Result***
**`Terminal`**
```
Hello, Will!
```

--- 

## Final Review

Thats it! To review

***Create a new C# console app ( in the current folder )***
```
dotnet new console --use-program-main
```

***Open your Program.cs in Visual Studio Code***
```
code Program.cs
```

***Build and Run your code***
```
dotnet build
dotnet run
```
