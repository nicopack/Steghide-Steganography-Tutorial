# Steghide Guide - Educational Purposes Only

## Disclaimer
This repository is for **educational purposes only**. I do **not condone any illegal activity**. Use this knowledge responsibly and within legal boundaries.

## Description
A step-by-step guide to using **Steghide**, a steganography tool for embedding and extracting hidden data within images. No installation required—just run it from the command line.

## Table of Contents
- [Download Steghide](#download-steghide)
- [Usage Guide](#usage-guide)
  - [Windows](#windows)
  - [Linux](#linux)
  - [MacOS](#macos)
- [Embedding Data](#embedding-data)
- [Extracting Data](#extracting-data)
- [Credits](#credits)

## Get Steghide
Download Steghide from the official site: [Steghide Download](https://steghide.sourceforge.net/download.php)
**OR**
Download it from this repository

## Usage Guide
### Windows
1. Download the **Windows binary** from the official website.
2. Extract the contents.
3. Navigate to the extracted folder in **Command Prompt**.
4. Run `steghide` commands as needed.

### Linux
1. Download the **Linux binary** from the official website.
2. Extract the files to your desired location.
3. Open **Terminal**.
4. Navigate to the Steghide directory.
5. Run `steghide` commands as needed.

### MacOS
1. Download the **MacOS binary** from the official website.
2. Extract the files.
3. Open **Terminal**.
4. Navigate to the Steghide directory.
5. Run `steghide` commands as needed.

## Embedding Data
1. Ensure you have a **.txt file** and preferably a **.bmp image**.
2. Navigate to the steghide directory/folder containing the cover image and the secret text:
   ```sh
   cd steghide
   ```
3. Run the following command to embed the text file into the image:
   ```sh
   steghide embed -cf cover.bmp -ef secret.txt
   ```
4. Enter a password when prompted (used for extraction later).

## Extracting Data
1. Navigate to the directory containing the stego-image:
   ```sh
   cd steghide
   ```
2. Run the following command to extract the hidden text file:
   ```sh
   steghide extract -sf cover.bmp
   ```
3. Enter the password used during embedding.
4. The extracted `secret.txt` file will appear in the directory.

## Credits
- [Steghide Official Website](https://steghide.sourceforge.net/)
