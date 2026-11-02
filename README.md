# FTC Link (Open Source)

FTC Link is an open-source plugin for Android Studio & IntelliJ IDEA developed by **Asteria Robotics (#32334)** to accelerate and simplify software development for FIRST Tech Challenge (FTC) teams.

> ** IMPORTANT NOTICE:**  
> This repository is maintained **strictly for source code inspection and review**.  
> Do **NOT** download the plugin binaries directly from this repository to install them. For the official release and automatic installation, please visit the **JetBrains Marketplace**.

---

## Installation & Usage

To install and use FTC Link in your IDE:

1. **Via JetBrains Marketplace (Recommended):**  
    [**Go to FTC Link on JetBrains Marketplace**](https://plugins.jetbrains.com/plugin/35570-ftc-link)

2. **Directly inside Android Studio / IntelliJ IDEA:**  
   Navigate to `Settings / Preferences` ➔ `Plugins` ➔ search for **"FTC Link"**, and click **Install**.

---

## Key Features

- **Gemini AI Assistant:** Ask technical questions, generate code snippets, and debug your Autonomous and TeleOp OpModes directly inside your workspace.
- **Instant OpMode Templates:** Generate pre-configured Java templates for Mecanum Drive, Swerve, Tank Drive, Limelight 3A, and AprilTag vision integration in seconds.
- **Dynamic Hardware Mapping:** Easily configure motor, servo, and sensor names through a dynamic UI panel.
- **Integrated Manual & Rule Search:** Quick reference to game manuals and constraints right within your IDE.

---

## Repository File Structure & Overview

This repository contains the core runtime components, dependencies, and artifacts for **FTC Link**:

* **`QuickManualAssistant-1.0.2-searchableOptions.zip`**
  * Indexing and search configuration data that allows Android Studio / IntelliJ IDEA to index FTC Link settings in the IDE Search bar (`Settings / Preferences`). If you don't want to download plugin from the plugin store, you can download this file.

* **`QuickManualAssistant-1.0.2.jar`**
  * The compiled Java Archive (JAR) containing the plugin's main application logic, UI components, and execution handlers.

* **`QuickManualAssistant-1.0.2.zip`**
  * The packaged distribution archive of the plugin, used for manual installation (`Install Plugin from Disk...`).

* **`README.md`**
  * Documentation file containing project info, feature highlights, and usage instructions.

* **`gson-2.10.1.jar`**
  * Google Gson library dependency used for parsing JSON data structures (e.g., API requests and responses from the Gemini AI Assistant).

* **`kotlinx-coroutines-swing-1.8.1.jar`**
  * Kotlin Coroutines Swing library providing asynchronous UI thread execution, ensuring the IDE interface remains responsive during background AI generation tasks.
