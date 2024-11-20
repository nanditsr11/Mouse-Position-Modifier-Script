#  Mouse Position Modifier Script

_Run it using PowerShell not as a Python file._

##   Description
This PowerShell script continuously modifies the position of the mouse cursor on the screen. It calculates new X and Y coordinates based on the cursor's current position, ensuring the cursor stays within a bounded region on the screen. The script repositions the cursor every second to demonstrate how mouse control can be achieved programmatically using the .NET Framework via PowerShell.

##  Purpose
The script can serve as a demonstration for:

- Programmatically controlling mouse movement.
- Learning about PowerShell scripting and .NET integration.
- Experimenting with user interface interactions or simulating mouse movement for testing purposes.

##  How It Works

1. Import Assembly
- The script uses the System. Windows.Forms assembly to access the mouse cursor's position and manipulate it.

2. Cursor Movement Logic

- The current mouse position is retrieved.
- A new position is calculated using a modulo operation to keep the X and Y coordinates within a 500x500 pixel boundary.
- The new position is adjusted by adding 100 pixels to avoid positioning the cursor too close to the screen edges.

3. Loop and Sleep

- The script runs indefinitely in a while ($true) loop.
- The Start-Sleep cmdlet pauses execution for 1 second between each repositioning.

##  Usage
1. Requirements:

- Windows OS.
- PowerShell 5.0 or later.
- .NET Framework installed.

2. Steps:

- Open a PowerShell terminal.
- Paste the script into the terminal.
- Run the script.

3. Stop the Script:

- Use Ctrl+C in the terminal to interrupt the loop.

##  Caution
- Running this script will interfere with normal mouse usage since it continuously moves the cursor.
- Make sure to test this in a safe environment where it will not disrupt critical tasks.
- The script can be stopped using the interrupt key (Ctrl+C).

##  Example

When you run the script, the cursor will jump around within a defined area on the screen, creating a "bounded jitter" effect. This can be useful for testing UI responsiveness or just for fun experimentation with programmatic cursor control.

##  License
This script is provided under the MIT License, which allows for free use, modification, and distribution with proper attribution.
