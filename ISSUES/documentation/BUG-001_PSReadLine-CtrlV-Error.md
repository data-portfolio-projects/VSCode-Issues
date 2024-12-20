# Bug: PSReadLine - Ctrl+V Paste Function Error

## Description:
When attempting to paste using `Ctrl+V` in the PowerShell terminal, the following error occurs:

Oops, something went wrong. Please report this bug with the details below.
Report on GitHub: https://github.com/lzybkr/PSReadLine/issues/new
-----------------------------------------------------------------------
Last 1 Keys:
Ctrl+v

Exception:
System.ArgumentOutOfRangeException: The value must be greater than or equal to zero and less than the console's buffer size in that dimension.
Parameter name: top
Actual value was -1.
   at System.Console.SetCursorPosition(Int32 left, Int32 top)
   at Microsoft.PowerShell.PSConsoleReadLine.ReallyRender(RenderData renderData, String defaultColor)
   at Microsoft.PowerShell.PSConsoleReadLine.ForceRender()
   at Microsoft.PowerShell.PSConsoleReadLine.Paste(Nullable`1 key, Object arg)
   at Microsoft.PowerShell.PSConsoleReadLine.ProcessOneKey(ConsoleKeyInfo key, Dictionary`2 dispatchTable, Boolean ignoreIfNoAction, Object arg)
   at Microsoft.PowerShell.PSConsoleReadLine.InputLoop()
   at Microsoft.PowerShell.PSConsoleReadLine.ReadLine(Runspace runspace, EngineIntrinsics engineIntrinsics)
