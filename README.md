# waw Unity CLI

## Overview

**waw Unity CLI** is a command-line tool designed to automate and manage **Unity platform configurations, builds, and project workflows**. It simplifies adding, removing, and handling multiple platforms for cross-platform Unity development.

## Installation

To install waw, which includes Unity CLI, use:

```
npm install -g waw
```

## Commands

### **Platform Management**

| Command                          | Description                                                                         |
| -------------------------------- | ----------------------------------------------------------------------------------- |
| `waw platform add <platform>`    | Adds a new platform to the project (e.g., `waw platform add vr-android`).           |
| `waw platform remove <platform>` | Removes an existing platform (e.g., `waw platform remove vr-android`).              |
| `waw platform open <platform>`   | Opens the platform's configuration in Unity (e.g., `waw platform open vr-android`). |
| `waw platform list`              | Lists all available platforms in the project.                                       |
| `waw platform init <platform>`   | Initializes platform-specific settings.                                             |
| `waw platform update <platform>` | Updates dependencies or configurations for a platform.                              |

### **Building Platforms**

| Command                | Description                                                   |
| ---------------------- | ------------------------------------------------------------- |
| `waw build <platform>` | Builds the specified platform (e.g., `waw build vr-android`). |
| `waw build all`        | Builds all configured platforms.                              |
| `waw clean`            | Cleans build files to free up space.                          |
| `waw status`           | Shows project status, including enabled platforms.            |

## Supported Platforms

| Name                | Platform Type | OS / Device                       |
| ------------------- | ------------- | --------------------------------- |
| **vr-android**      | VR            | Quest, Pico (Standalone VR)       |
| **vr-windows**      | VR            | Valve Index, HTC Vive, Windows MR |
| **vr-macos**        | VR            | Mac-compatible VR (limited)       |
| **mobile-android**  | Mobile        | Android phones & tablets          |
| **mobile-ios**      | Mobile        | iPhones & iPads                   |
| **desktop-windows** | Desktop       | Windows PC                        |
| **desktop-linux**   | Desktop       | Linux PC                          |
| **desktop-macos**   | Desktop       | Mac                               |
| **web**             | Web           | WebGL & WebXR (Browsers)          |

## Example Usage

```sh
# Add a new platform
waw platform add vr-android

# Remove a platform
waw platform remove vr-android

# Open platform configuration
waw platform open vr-android

# Build for a specific platform
waw build vr-android

# Build all configured platforms
waw build all
```

## Next Steps

- Ensure **waw CLI** is installed and configured.
- Add, configure, and build platforms as needed.
- Automate workflows with **CI/CD integration**.

🚀 **waw Unity CLI makes cross-platform Unity development fast and efficient!**

