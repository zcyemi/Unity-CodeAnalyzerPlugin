# Unity-CodeAnalyzerPlugin
Untiy plugin for integrating any roslyn code analyzer dll with VisualStudio or VSCode.

## What is Unity-CodeAnalyzerPlugin

Unity will regenerate csproj file after any script file changes. 
The analyzer reference which manually attatched to Unity's .csproj will be reverted automatically.

This plugin hook the .csproj refreshing process and insert the analyzer reference into .csproj file if missing.

## Quick Start

1. Copy the [folder](https://github.com/soyemi/Unity-CodeAnalyzerPlugin/tree/master/Assets) to your unity project asset path.
2. Click menu item `CodeAnalysis/Config`, then select custom analyzer dll.
3. Click menu item `CodeAnalysis/Refresh`, apply the analyzer to csproj.
4. double-click any script asset, open source file in Visual Studio. The selected analyzer appears on the `slution window/<Project>/references/analyzer/`.

## Other

Alternatives: [UnityEngineAnalyzer](https://github.com/meng-hui/UnityEngineAnalyzer)

feature
- Visual Studio editor code analysis.
- VSCode partially supported. use cli command `msbuild build` to get all diagnostics on console.
- No need to install vsix.
