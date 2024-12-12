

# FFmpeg Installation Guide

This guide will walk you through the process of installing FFmpeg on both **Windows** and **Linux** systems. FFmpeg is a powerful multimedia framework for handling video, audio, and other multimedia files and streams.

## Table of Contents
- [Installing FFmpeg on Windows](#installing-ffmpeg-on-windows)
- [Installing FFmpeg on Linux](#installing-ffmpeg-on-linux)



### Installing FFmpeg on Windows

1. **Download FFmpeg for Windows**
   - Visit the official FFmpeg website: [https://ffmpeg.org/download.html](https://ffmpeg.org/download.html)
   - Scroll down to the "Windows" section and click on the link to the **Windows builds by BtbN** or **Gyan** (both are trusted sources for Windows builds).
   - On the chosen page, find the latest build and download the zip file (e.g., `ffmpeg-release-i686-static.zip`).

2. **Extract the Downloaded Archive**
   - After downloading, locate the zip file and extract it using a tool like WinRAR or 7-Zip.
   - Right-click on the zip file and select "Extract All..." or use 7-Zip's "Extract here" option.

3. **Move FFmpeg to a Convenient Location**
   - Once extracted, move the extracted folder (e.g., `ffmpeg-2024-12-07` or similar) to a convenient location, such as `C:\ffmpeg\`.

4. **Add FFmpeg to the System Path**
   - Open the **Start Menu** and search for `Environment Variables`.
   - Select **Edit the system environment variables**.
   - In the **System Properties** window, click on **Environment Variables**.
   - Under **System variables**, find the **Path** variable and click **Edit**.
   - In the **Edit Environment Variable** window, click **New** and add the path to the `bin` directory inside the FFmpeg folder. For example:
     ```
     C:\ffmpeg\bin
     ```
   - Click **OK** to save your changes.

5. **Verify Installation**
   - Open **Command Prompt** (`cmd`) and type the following command:
     ```
     ffmpeg -version
     ```
   - If FFmpeg is correctly installed, you should see the version information printed to the screen.



### Installing FFmpeg on Linux

The steps for installing FFmpeg on Linux may vary slightly depending on the distribution you're using. Below are instructions for **Ubuntu/Debian-based** distributions and **Fedora**.

#### For Ubuntu/Debian-based Systems

1. **Update Package List**
   - Open a terminal and run the following command to update the package list:
     ```bash
     sudo apt update
     ```

2. **Install FFmpeg**
   - Install FFmpeg using the following command:
     ```bash
     sudo apt install ffmpeg
     ```

3. **Verify Installation**
   - Once the installation is complete, verify FFmpeg installation by running:
     ```bash
     ffmpeg -version
     ```
   - You should see FFmpeg version details displayed on the terminal.

#### For Fedora-based Systems

1. **Install FFmpeg**
   - First, enable the RPM Fusion repository, which contains FFmpeg packages:
     ```bash
     sudo dnf install https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm
     ```

2. **Install FFmpeg**
   - Now install FFmpeg using the following command:
     ```bash
     sudo dnf install ffmpeg
     ```

3. **Verify Installation**
   - After installation, confirm FFmpeg is working by checking its version:
     ```bash
     ffmpeg -version
     ```

#### For Arch Linux

1. **Install FFmpeg**
   - Open a terminal and run:
     ```bash
     sudo pacman -S ffmpeg
     ```

2. **Verify Installation**
   - Check FFmpeg’s installation:
     ```bash
     ffmpeg -version
     ```



### Additional Notes

- **Windows**: If you encounter issues with FFmpeg not being recognized, make sure that the `bin` directory is correctly added to your system path and restart the terminal or Command Prompt.
- **Linux**: On some Linux distributions, FFmpeg might not be available in the default repositories. You can build it from source or use a third-party repository like **FFmpeg's official website** for detailed instructions on building from source.



Now you have FFmpeg installed and ready to use on your system!

