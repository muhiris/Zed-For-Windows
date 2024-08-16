# Zed for Windows

Welcome! This guide provides clear steps to install the **Zed Code Editor**. The official documentation was difficult to follow, so I created this simplified version.

## Installation Steps

1. **Download Rust Init** from:

    [Download  rustup-init.exe  (64-bit)](https://static.rust-lang.org/rustup/dist/x86_64-pc-windows-msvc/rustup-init.exe)

2. Open the downloaded **rustup-init.exe** file. When prompted, choose **1. Default Installation**.

3. After installation, verify it by opening a new terminal and typing:

    ```bash
    rustup
    ```

    If you see information about the **rustup** command, the installation was successful.

4. Clone the Zed repository:

    ```bash
    git clone https://github.com/zed-industries/zed.git
    ```

5. Navigate to the cloned folder:

    ```bash
    cd zed
    ```

6. Run the application:

    ```bash
    cargo run --release
    ```

    You have now successfully installed Zed!

## Build Issues

Ensure you have the following:

- **Visual Studio**
- **GitHub CLI**
- **rustup**

Try following work around for any of these issues
 
    
    rustup update
    rustup target add wasm32-wasi
    

Installing [Visual Studio Community](https://visualstudio.microsoft.com/downloads/) 

Installing the Windows 11 or 10 SDK, ensuring at least `Windows 10 SDK version 2104 (10.0.20348.0)` is installed. Download it from the [Windows SDK Archive](https://developer.microsoft.com/windows/downloads/windows-sdk/).