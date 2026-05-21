# ZenVersion

Remote version file for the **Zen** Gorilla Tag mod update checker.

This repo only holds `PluginInfo.cs`. The game mod reads it on startup and compares it to the version you have installed.

## How it works

1. Zen downloads: https://raw.githubusercontent.com/yourlocalrifty/ZenVersion/main/PluginInfo.cs
2. It reads the `Version` string in that file.
3. If GitHub's version is newer than your installed mod, you get an outdated warning in-game.

## File

```csharp
namespace Zen
{
 public static class PluginInfo
 {
     public const string GUID = "com.skye.zen";
     public const string Name = "Zen";
     public const string Version = "1.0.0";
 }
}
