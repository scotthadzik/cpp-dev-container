# CS Class C++ Dev Container

This repository contains the VS Code Dev Container configuration for our C++ class. It gives everyone the same development environment with the full desktop VS Code app.

**What is included inside the container:**
- g++ and gcc compiler
- gdb debugger
- make and cmake build tools
- valgrind memory checker
- C/C++ IntelliSense extension (auto-installed)
- CMake Tools extension (auto-installed)

---

## One-Time Setup (Do This Once)

### Step 1 - Install Docker Desktop
Download and install Docker Desktop for your operating system:
https://www.docker.com/products/docker-desktop/

After installing, open Docker Desktop and let it finish starting up. You will see a whale icon in your taskbar or menu bar when it is ready. You do not need to do anything else in Docker Desktop - just keep it running in the background.

### Step 2 - Install VS Code
If you do not already have it:
https://code.visualstudio.com/

### Step 3 - Install the Dev Containers Extension
1. Open VS Code
2. Click the Extensions icon on the left sidebar (or press Ctrl+Shift+X)
3. Search for: Dev Containers
4. Install the extension published by Microsoft

### Step 4 - Download This Repository
Click the green Code button at the top of this page, then choose Download ZIP. Extract it to a folder on your computer (for example, your Documents folder).

---

## Opening the Dev Container

1. Open VS Code
2. Go to File then Open Folder and select the folder you extracted
3. VS Code will show a popup in the bottom-right corner: "Reopen in Container" - click it
   - If you miss the popup: press Ctrl+Shift+P, type Reopen in Container, and press Enter
4. Wait for the container to build - this takes about 2-3 minutes the first time only
5. Once it opens, you are ready to code! Open a terminal with Ctrl and the backtick key and try: g++ --version

Note for Apple Silicon Mac users (M1/M2/M3): Make sure you download the Apple Silicon version of Docker Desktop.

---

## Compiling and Running C++

Open the built-in terminal (Ctrl + backtick) and use standard g++ commands:

    # Compile
    g++ -o myprogram myfile.cpp

    # Run
    ./myprogram

    # Compile with debugging info
    g++ -g -o myprogram myfile.cpp

---

## Troubleshooting

**Reopen in Container popup did not appear**
Press Ctrl+Shift+P, type Reopen in Container, and press Enter.

**Container fails to build or Docker errors**
Make sure Docker Desktop is open and fully started (whale icon in taskbar). Then try again.

**VS Code says Docker not found**
Restart VS Code after installing Docker Desktop.

**Container is slow the first time**
This is normal - it is downloading and building the image. Subsequent opens are fast.
