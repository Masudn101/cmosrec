# cmosrec

Sure! To select **option 2** in a batch script automatically (for example, if you’re referring to a command line utility that prompts for options), you can simulate input by using `echo` and piping it into the command.

Here’s how you can modify the script to automatically select **option 2** for `cmospwd_win.exe /k`:

### Updated Windows Batch Script:

```batch
@echo off

REM Running ioperm -i (Assuming you have ioperm.exe available in your PATH or current directory)
ioperm.exe -i

REM Automatically selecting option 2 for cmospwd_win.exe /k
echo 2 | cmospwd_win.exe /k

pause
```

### Explanation:
- `echo 2 |` sends the number `2` as input to `cmospwd_win.exe /k`, simulating that you're choosing option 2 in the menu prompt.

### Instructions:
- Place this script in a `.bat` or `.cmd` file.
- Make sure that `ioperm.exe` and `cmospwd_win.exe` are accessible (either in the same directory or in the system's PATH).
- Run the batch file, and it should automatically select option 2 when `cmospwd_win.exe /k` is executed.

Let me know if you need further assistance!




























