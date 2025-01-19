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

1. Launch the Electron app.
2. Use the graphical interface to send commands to the Kali Linux system.
3. View results directly in the app or through your terminal.

## Screenshot
1. ![image](https://github.com/user-attachments/assets/f872c474-2ae7-4cf6-aa6b-5854897af1dc)
2. ![image](https://github.com/user-attachments/assets/757243ea-20ac-4846-9a00-f1cd7ab241ee)
3. ![image](https://github.com/user-attachments/assets/42d5cb50-52fb-4cb8-9070-7e105cc8d836)
4. ![image](https://github.com/user-attachments/assets/d955a3c5-79e9-41c4-9d0e-25a96f12f301)
5. ![image](https://github.com/user-attachments/assets/cf38ac1c-430f-462e-a4d7-07646f3e8089)






