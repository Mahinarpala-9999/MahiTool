# MahiTool

## Overview

MahiTool is a powerful utility designed to integrate an Electron app with Python scripts running on Kali Linux. It facilitates advanced remote access and cybersecurity operations by providing a seamless interface to execute Python commands and automate tasks on Kali Linux.

## Features

- **Remote Command Execution**: Execute Python commands on a Kali Linux system through the Electron app.
- **Cross-Platform Compatibility**: Provides a user-friendly interface that runs on multiple platforms.
- **Modular Design**: 
  - `main.js`: Handles Electron functionality and interfaces with the backend.
  - `main.py`: Runs backend commands on Kali Linux for task automation.
- **Simplified Workflow**: Automates tasks using a graphical interface.

## Project Structure

```plaintext
mahi-tool/
├── main.js             # Core functionality for the Electron app.
├── main.py             # Python script for backend commands on Kali Linux.
├── package.json        # Configuration file for the Electron project.
├── package-lock.json   # Automatically generated file to ensure consistent dependencies.
└── screenshot.png      # Visual representation of the app's interface.
```

## Prerequisites

Ensure the following dependencies are installed before running the project:

- **Node.js** (v16 or later)
- **Python** (v3.8 or later)
- **Kali Linux**

## Installation

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/Mahinarpala-9999/mahi-tool.git
   cd mahi-tool
   ```

2. Install the required dependencies:

   ```bash
   npm install
   ```

3. Run the Electron app:

   ```bash
   npm start
   ```

4. Ensure `main.py` is executable and properly configured for your Kali Linux environment.

## Usage

1. **Launch the Electron App**: Once the app is launched, it will communicate with the backend running on Kali Linux.
2. **Execute Remote Commands**: You can send commands from Firebase to execute on the Kali Linux system. The app can run commands like `device info`, `take screenshot`, `upload media files`, etc.
3. **Upload Media Files**: The app supports uploading various types of media to a server for storage and further analysis.
4. **System Information**: The app can gather device information (like OS version, hardware specs, etc.) and upload it to Firebase or a specified server.
5. **Proxy Functionality**: The app will route the device's internet traffic through a proxy server, masking the real IP address for anonymity.

### Example Commands

- **Device Info**: Retrieve and upload system information to Firebase:
  ```bash
  firebase.database().ref('commands/device_info').set({
      status: 'run',
      action: 'get_device_info'
  });
  ```

- **Take Screenshot**: Capture and upload a screenshot to the server:
  ```bash
  firebase.database().ref('commands/take_screenshot').set({
      status: 'run',
      action: 'capture_screenshot'
  });
  ```

- **Upload Media**: Upload an image file to the server:
  ```bash
  firebase.database().ref('commands/upload_media').set({
      status: 'run',
      action: 'upload_image',
      file: 'image_path'
  });
  ```

## Proxy Implementation

This project includes functionality for IP masking by using a proxy server. The app connects to a proxy server and routes its internet traffic, ensuring that the real IP address is hidden.

### Steps for Proxy Setup

1. **Login to the server**: The proxy server is controlled by the login credentials.
2. **Execute Proxy Change**: When the Expo app connects to the server, it uses the proxy IP from the `login.txt` file stored on the server.


## Screenshot
1. ![image](https://github.com/user-attachments/assets/f872c474-2ae7-4cf6-aa6b-5854897af1dc)
2. ![image](https://github.com/user-attachments/assets/757243ea-20ac-4846-9a00-f1cd7ab241ee)
3. ![image](https://github.com/user-attachments/assets/42d5cb50-52fb-4cb8-9070-7e105cc8d836)
4. ![image](https://github.com/user-attachments/assets/d955a3c5-79e9-41c4-9d0e-25a96f12f301)
5. ![image](https://github.com/user-attachments/assets/cf38ac1c-430f-462e-a4d7-07646f3e8089)


## Disclaimer

This tool is intended for educational and ethical hacking purposes only. It should only be used in environments where explicit permission has been granted. Unauthorized use of this tool could be illegal and unethical. Always ensure you have permission before using this tool on any system.


***for server files to upload the all documents contact me ***



