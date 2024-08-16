# Zed for Windows

Welcome! This guide provides clear steps to install the **Zed Code Editor**. The official documentation was difficult to follow, so I created this simplified version.

## Installation Steps

1. **Download Rust Init** from:

    [Download rustup-init.exe (64-bit)](https://static.rust-lang.org/rustup/dist/x86_64-pc-windows-msvc/rustup-init.exe)

2. Open the downloaded **rustup-init.exe** file. When prompted, choose **1. Default Installation**.

3. After installation, verify it by opening a new terminal and typing:

    ```bash
    rustup
    ```

    If you see information about the **rustup** command, the installation was successful.

4. **Download and Install Build Tools**:

    Download the Visual Studio Build Tools installer from:

    [Download vs_BuildTools.exe](https://aka.ms/vs/17/release/vs_BuildTools.exe)

    Run the installer and select the following components:
    - **MSVC v143 - VS 2022 C++ x64/x86 build tools**
    - **Windows 10 SDK (10.0.18362)**
    - **C++ CMake tools for Windows**
    
    Complete the installation process.

5. **Install the Windows SDK**:

    Make sure you have at least `Windows 10 SDK version 2104 (10.0.20348.0)` installed. You can download the latest version of the Windows SDK from:

    [Windows SDK Archive](https://developer.microsoft.com/en-us/windows/downloads/windows-sdk/)

6. **Clone the Zed repository**:

    ```bash
    git clone https://github.com/zed-industries/zed.git
    ```

7. **Navigate to the cloned folder**:

    ```bash
    cd zed
    ```

8. **Run the application**:

    ```bash
    cargo run --release
    ```

    You have now successfully installed Zed!

## Build Issues

Ensure you have the following:

- **Visual Studio Build Tools** (or Visual Studio Community)
- **GitHub CLI**
- **rustup**

If you encounter build issues, try the following workarounds:

1. Update Rust and add the WebAssembly target:

    ```bash
    rustup update
    rustup target add wasm32-wasi
    ```

2. Verify your installation of the Windows SDK and ensure that the correct version is installed.
