# Mod Maker – MSC Mod Template

Mod Maker is a simple template for creating *My Summer Car* mods. Quickly set up your mod and start coding without worrying about .NET issues.

## Requirements
- .NET Framework 3.5  
- Visual Studio 2017/2022/2026  
- Basic C# knowledge  

## Getting Started
1. Create a Class Library (.NET Framework 3.5) project.  
2. Add references from your MSC folder:  
   - Assembly-CSharp  
   - MSCLoader  
   - PlayMaker  
   - UnityEngine  
   - UnityEngine.UI  
3. Rename your class and set:  
   - `ID` – unique mod identifier  
   - `Name` – your mod name  
   - `Author` – your name  
   - `Version` – e.g., `1.0`  
   - `Description` – short description  
4. Add code in `ModSetup()`, `Mod_OnLoad()`, and `Mod_Settings()`.  
5. Build and place the `.dll` in `MSCLoader/Mods`.  

## Tips
- Keep `ModID` unique  
- Avoid class and variable name conflicts  

## License
MIT

you will see everything in the code.
