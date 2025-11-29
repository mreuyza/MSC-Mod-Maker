# Mod Maker – MSC Mod Template

Easily create *My Summer Car* mods with this starter template. Set your mod ID, name, author, version, and start coding.  

## Requirements
- .NET Framework 3.5  
- Visual Studio 2017/2022/2026  

## Quick Start
1. Create a Class Library (.NET Framework 3.5)  
2. Add references: Assembly-CSharp, MSCLoader, PlayMaker, UnityEngine, UnityEngine.UI  
3. Rename class and set ID, Name, Author, Version, Description  
4. Add code in ModSetup(), Mod_OnLoad(), Mod_Settings()  
5. Build and drop `.dll` in MSCLoader/Mods  

Keep ModID unique and avoid naming conflicts.
