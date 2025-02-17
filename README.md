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
| `waw build clean`      | Cleans build files to free up space.                          |
| `waw status`           | Shows project status, including enabled platforms.            |

### **Scene Management**

| Command                   | Description                                                           |
| ------------------------- | --------------------------------------------------------------------- |
| `waw scene add <name>`    | Creates a new scene from a template (e.g., `waw scene add MainMenu`). |
| `waw scene remove <name>` | Deletes an existing scene from the project.                           |
| `waw scene save <name>`   | Saves the current scene as a template for future reuse.               |
| `waw scene fetch <name>`  | Retrieves a saved scene template and adds it to the project.          |

### **Model Management**

| Command                   | Description                                                 |
| ------------------------- | ----------------------------------------------------------- |
| `waw model add <name>`    | Adds a 3D model from a shared asset library.                |
| `waw model remove <name>` | Deletes a model from the project.                           |
| `waw model save <name>`   | Saves a model to a reusable template library.               |
| `waw model fetch <name>`  | Retrieves a model template and imports it into the project. |

### **Prefab Management**

| Command                    | Description                                          |
| -------------------------- | ---------------------------------------------------- |
| `waw prefab add <name>`    | Adds a prefab to the project from a shared template. |
| `waw prefab remove <name>` | Deletes a prefab from the project.                   |
| `waw prefab save <name>`   | Saves a prefab as a template for reuse.              |
| `waw prefab fetch <name>`  | Retrieves a prefab from a shared library.            |

### **Material Management**

| Command                      | Description                            |
| ---------------------------- | -------------------------------------- |
| `waw material add <name>`    | Adds a material from a shared library. |
| `waw material remove <name>` | Deletes a material from the project.   |
| `waw material save <name>`   | Saves a material for reuse.            |
| `waw material fetch <name>`  | Retrieves a saved material template.   |

### **Audio Management**

| Command                   | Description                         |
| ------------------------- | ----------------------------------- |
| `waw audio add <name>`    | Adds an audio file to the project.  |
| `waw audio remove <name>` | Deletes an audio file.              |
| `waw audio save <name>`   | Saves an audio asset as a template. |
| `waw audio fetch <name>`  | Retrieves a saved audio asset.      |

### **Script Management**

| Command                    | Description                          |
| -------------------------- | ------------------------------------ |
| `waw script add <name>`    | Adds a script from a shared library. |
| `waw script remove <name>` | Deletes a script from the project.   |
| `waw script save <name>`   | Saves a script for reuse.            |
| `waw script fetch <name>`  | Retrieves a saved script template.   |

### **UI Layout Management**

| Command                | Description                              |
| ---------------------- | ---------------------------------------- |
| `waw ui add <name>`    | Adds a UI layout from a shared template. |
| `waw ui remove <name>` | Deletes a UI layout.                     |
| `waw ui save <name>`   | Saves a UI layout for reuse.             |
| `waw ui fetch <name>`  | Retrieves a saved UI layout.             |

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
