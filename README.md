# Code App

Bringing desktop-like editing experience to iPad, available on [App Store](https://apps.apple.com/us/app/code-app/id1512938504) and [TestFlight](https://testflight.apple.com/join/EgZ8sE2P).

![Code App Screenshot](https://thebaselab.com/code/clang.png)

## About the repository

This repository contains the source code of the app. We also work on issues, listen to your feedback and publish our development plan here.

## Documentation

See [code.thebaselab.com](https://code.thebaselab.com)

## The Plan

Use [VS Code](https://github.com/microsoft/vscode) as a design template while providing key functionalities with [monaco-editor](https://github.com/microsoft/monaco-editor) and native code:

- Version Control (Git clone, commits, diff editor, push, pull and gutter indicator) ✅
- Embedded terminal (70+ commands available) ✅
- Local web development environment (Node + PHP) ✅
- Built in Python runtime ✅
- C/C++ Runtime with WebAssembly (with clang) ✅
- Local Java (OpenJDK) ✅
- SSH Support ✅
- [LSP](https://microsoft.github.io/language-server-protocol) support (Python & Java) ✅ 

## Building the project

1. `git clone https://github.com/thebaselab/codeapp`
2. `./downloadFrameworks.sh`
3. Open Code.xcodeproj
4. Switch to CodeUI target if you wish to run the app on a simulator
5. Click build

## Running on an iPhone

1. Install the latest Xcode version (or Xcode beta) that supports your iOS version.
2. Clone this repository and run `./downloadFrameworks.sh`.
3. Open `/home/runner/work/codeapp/codeapp/Code.xcodeproj` in Xcode.
4. In **Signing & Capabilities** for the app target:
   - Set a unique **Bundle Identifier**.
   - Select your **Apple Developer Team**.
5. Connect your iPhone, unlock it, trust the Mac, and enable **Developer Mode** on iPhone.
6. Select your iPhone as the run destination in Xcode, then build and run.

## Distribution (TestFlight / App Store)

1. Use a paid Apple Developer account.
2. Archive the app in Xcode.
3. Upload the archive to App Store Connect.
4. Distribute through TestFlight or submit to the App Store.

> If Xcode does not recognize your iOS version, update to a newer Xcode release or beta.

The source code of the built-in languages are hosted on these repositories.
| Language | Repository |
|-----------------|-------------------|
| Python 3.9.2 | [cpython](https://github.com/holzschu/cpython/tree/3.9)|
| Clang 14.0.0 | [llvm-project](https://github.com/holzschu/llvm-project)|
| PHP 8.3.2 | [php-src](https://github.com/bummoblizard/php-src/tree/PHP-8.3.2)|
| Node.js 18.19.0 | [nodejs-mobile](https://github.com/1Conan/nodejs-mobile)|
| OpenJDK 8 | [android-openjdk-build-multiarch](https://github.com/thebaselab/android-openjdk-build-multiarch)|
