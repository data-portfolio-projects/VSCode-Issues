# Known Bugs in VS Code

## Issue: Pasting Crashes VS Code
**Description:** Pasting content into the editor causes a crash.
**Steps to Reproduce:**
1. Open VS Code.
2. Press `Ctrl+v` to paste text into the editor.
3. VS Code crashes immediately.
**Cause:** The bug appears to be related to an extension or internal rendering issue.
**Resolution:**
- Try disabling extensions related to clipboard management.
- Update the `PSReadLine` module if using PowerShell integrated terminal.
- Report the issue on the [VS Code GitHub Repository](https://github.com/Microsoft/vscode).

## Issue: Extension Not Loading
**Description:** Extensions are not loading after updating VS Code.
**Steps to Reproduce:**
1. Update VS Code to the latest version.
2. Restart the IDE and check the extensions panel.
3. Extensions fail to load.
**Cause:** A recent update may have caused a conflict between extensions.
**Resolution:**
- Disable all extensions and re-enable them one by one to identify the conflicting one.
- Check the VS Code logs for errors related to extension loading.
