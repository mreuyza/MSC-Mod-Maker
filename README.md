
NOTE:This is a code tooked from the mscloader template for those who .net framework doesn't working inside the template,or just want to start modding MSC


To do this you would need these things:
.NET FrameWork 3.5
Visual Studio 2017/2022/2026 or some of that
Also when you install some of the visual studio version you need to look down right to see Solution Explorer(you need to click it to start the work.)
Now Follow the instructions down below

First off create a class:

Create a new project

Click alt+s or click search for templates

Search for Class Libary

Find Class Library (.NET Framework)

Make sure to select .NET Framework 3.5 (or else it wont work)

Make a Name

Click Create

Second add references

Right click on References and then click Add Reference

Click Browse

Go to your game location in example

X:\My Summer Car\mysummercar_Data\Managed

Add these:

Assembly-CSharp
MSCLoader
PlayMaker
UnityEngine
UnityEngine.UI

(If you want add UnityEngine.UI i just add these so i am sure i dont skip some references)


Third Code

Click Class1.cs and paste this code:
 
 
using System;
using MSCLoader;
using UnityEngine;

public class NameMod : Mod -
{
	private GameObject NameMod; - Make Sure its not the same as public class NameMod because you will get errors

	public override string ID => "YourModID"; - ModID (this is very important so make sure you fill this)

	public override string Name => "Mod Name"; - Your Mod Name

	public override string Author => "Your Name"; - Your Name

	public override string Version => "1.0"; - Version

	public override string Description => ""; - Description

	public override void ModSetup()
	{

	}

	private void Mod_Settings()
	{
	}

	private void Mod_OnLoad()
	{

	}
}

It should look something like this:

using System;
using MSCLoader;
using UnityEngine;

public class NameMod : Mod 
{
    private GameObject NameMod;

    public override string ID => "YourModID";

    public override string Name => "Mod Name";

    public override string Author => "Your Name";

    public override string Version => "1.0"; 

    public override string Description => ""; 

    public override void ModSetup()
    {

    }

    private void Mod_Settings()
    {
    }

    private void Mod_OnLoad()
    {

    }
}


Tips •ᴗ•

For the YourmodID its more for assets,like my tripo plushie mod,you will need this,its important in anyway.When its a only .dll file you dont need to create an asset folder

Make sure to share this with someone who wants to start modding.

I'll put a template .vsix extractor(and if it has some errors like when joining game and see your mod is not working read it and see if its because of the framework,then read 1.)

Have a great day


⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣀⣤⣤⣤⣤⣤⣤⣀⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⢀⣠⣶⠿⠛⠉⠉⠁⠀⠀⠀⠉⠉⠛⠻⢶⣤⡀⠀⠀⠀⠀⠀
⠀⠀⠀⢀⣴⠟⠋⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀ ⠀⠉⠻⣦⣀⠀⠀⠀
⠀⠀⣰⡿⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀ ⠈⢻⣦⠀⠀
⠀⣼⡟⠀⠀⠀⠀⣀⣤⣄⡀⠀⠀⠀⠀⠀⠀⠀⣀⣤⣀⠀⠀⠀⠀⠹⣷⠀
⢰⡟⠀⠀⠀⠀⢸⣿⣿⣿⣷⠀⠀⠀⠀⠀⠀⣾⣿⣿⣿⣷⠀⠀⠀⠀⢹⣇
⣿⠇⠀⠀⠀⠀⠘⠿⣿⡿⠏⠀⠀⠀⠀⠀⠀⠙⢿⣿⡿⠋⠀⠀⠀⠀⠈⣿
⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀  ⣿
⣿⡇⠀⠀⠀⠀⣠⣤⣶⣶⠶⠶⠶⠶⠶⠶⠶⠶⢶⣶⣦⣤⠀⠀⠀⠀⢀⣿
⠸⣧⠀⠀⠀⠀⢿⣇⠀⠀⠀⠀⣀⣀⣀⡀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀ ⣸⡏
⠀⢻⣧⠀⠀⠀⠘⢿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠃⠀⠀⠀⣰⡿⠀
⠀⠀⠻⣧⡀⠀⠀⠈⠛⢿⣿⣿⣿⣿⣿⣿⣿⣿⡿⠟⠁⠀⠀⢀⣴⡟⠁⠀
⠀⠀⠀⠈⠻⣦⣀⠀⠀⠀⠈⠉⠉⠛⠛⠉⠉⠁⠀⠀⠀⢀⣴⡿⠋⠀⠀⠀
⠀⠀⠀⠀⠀⠈⠛⠷⣦⣄⣀⣀⠀⠀⠀⠀⢀⣀⣠⣴⡾⠟⠉⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠉⠙⠛⠛⠛⠛⠛⠛⠋⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀


this is the same as in the mod maker
(the mod maker.txt file is made so you can close this and learn from the .txt)
