# Clickable Button Hints

Makes hint buttons in VSCode clickable.

[Demo](https://user-images.githubusercontent.com/43412083/136652967-82e3fc07-8346-45a2-abd5-fa5f084440d2.mp4)

### **SPECIAL NOTE: If Visual Studio Code complains about being corrupted, simply click “Don't show again”.**

![Screenshot 2021-10-09 135923](https://user-images.githubusercontent.com/43412083/136652736-79c70528-acd5-470a-874a-aa8af273818d.png)

### **NOTE: Every time after Visual Studio Code is updated, please re-enable Custom CSS.**

### **NOTE: Every time you change the configuration, please re-enable Custom CSS.**

### **Starting from extension version 6.0, to be compatible with VSCode 1.58, the CSS/JS files being applied will be inlined into VSCode's workbench.**

Based on [be5invis](https://github.com/be5invis)’s [vscode-custom-css](https://github.com/be5invis/vscode-custom-css).

## Getting Started

1. Install this extension.

2. Restart Visual Studio Code with proper permission to modify itself:

   - **Windows**: Restart with Administrator Permission.

   - **MacOS and Linux**: See instructions below.

3. Activate command "Enable clickable button hints".

4. Restart.

## Extension commands

As you know to access the command palette and introduce commands you can use **_F1_** (all OSes), **_Ctrl+Shift+P_** (Windows & Linux) or **_Cmd+Shift+P_** (OS X).

- **_Enable clickable button hints_**: It enables clickable button hints, by injecting a bit of CSS.

- **_Disable clickable button hints_**: It will disable custom CSS.
- **_Reload clickable button hints_**: Disable and then re-enable it.

## Windows users

**In Windows, make sure you run your Visual Studio Code in Administrator mode before enabling or disabling your custom style!**

## Mac and Linux users

**The extension would NOT if Visual Studio Code cannot modify itself.** The cases include:

- Code files being read-only, like on a read-only file system or,
- Code is not started with the permissions to modify itself.

**You need to claim ownership on Visual Studio Code's installation directory, by running this command**:

```sh
sudo chown -R $(whoami) <Path to Code>
```

The placeholder `<Path to Visual Studio Code>` means the path to VSCode installation. It is typically:

- `/Applications/Visual Studio Code.app/Contents/MacOS/Electron`, on MacOS;
- `/Applications/Visual Studio Code - Insiders.app/Contents/MacOS/Electron`, on MacOS when using Insiders branch;
- `/usr/share/code`, on most Linux;
- `/usr/lib/code/` or `/opt/visual-studio-code` on Arch Linux.

Mac and Linux package managers may have customized installation path. Please double check your path is correct.

## Disclaimer

This extension modifies some Visual Studio Code files so use it at your own risk.
Currently, icons are not supported by the extension functionality that Visual Studio Code provides so this extension solves this issue by injecting code into:

- `electron-browser/index.html`.

The extension will keep a copy of the original file in case something goes wrong. That's what the disable command will do for you.

As this extension modifies Visual Studio Code files, it will get disabled with every Visual Studio Code update. You will have to enable icons again via the command palette.

**Please, leave a review if you can, so the Visual Studio Code Team can know that this is a very demanded feature and, maybe, they can then provide a proper way to extend the IDE regarding icons and customizations soon enough. ;D**

## Credits

Huge thanks to [be5invis](https://github.com/be5invis) for creating a really clean and simple base for me to build upon, and [Roberto Huertas](https://twitter.com/robertohuertasm) for coming up with [vscode-icons](https://github.com/vscode-icons/vscode-icons).
