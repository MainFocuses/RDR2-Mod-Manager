

# Voidz Mod Loader HTA

## Overview
Voidz Mod Loader HTA is a simple tool designed to facilitate copying and deleting files and folders between specified source and destination directories. It utilizes a configuration file (`loc.cfg`) to manage these directories.

## Features
- **Copy Files**: Copies all files and subdirectories from the source folder to the destination folder.
- **Delete Files**: Deletes files and folders in the destination folder that have the same names as those in the source folder.
- **Open Source Folder**: Opens the Windows Explorer window for the source folder.
- **Open Destination Folder**: Opens the Windows Explorer window for the destination folder.
- **Read and Refresh Config**: Reloads the configuration file (`loc.cfg`) to update source and destination folders.

## Getting Started
1. **Configuration Setup**:
   - Ensure the `loc.cfg` file is correctly configured with the paths to your source and destination folders. The format should be:
     ```
     source=path\to\source\folder
     destination=path\to\destination\folder
     ```
   - Example:
     ```
     source=C:\Users\Username\Documents\Mods
     destination=D:\Games\MyGame\Mods
     ```

2. **Running the Script**:
   - Double-click on `VoidzModLoader.hta` to open the application.
   - Upon startup, a message box will appear indicating the version of the script.

3. **Using the Interface**:
   - **Copy Files**: Clicking this button will copy all files and subdirectories from the source folder to the destination folder. A message box will confirm completion.
   - **Delete Files**: Clicking this button will delete files and folders in the destination folder that have the same names as those in the source folder. A message box will confirm completion.
   - **Open Source Folder**: Opens Windows Explorer for the source folder.
   - **Open Destination Folder**: Opens Windows Explorer for the destination folder.
   - **Read and Refresh Config**: Reloads the configuration file to update the source and destination folders. This is useful if you've edited the `loc.cfg` file manually and want to apply the changes without restarting the script.

4. **Error Handling**:
   - If the source or destination folder paths are incorrect or missing in the `loc.cfg` file, error messages will appear, and the script may close.

5. **Notes**:
   - Ensure that the folders specified in `loc.cfg` exist and are accessible.
   - This script uses VBScript and HTML Application (HTA) format, which may require Internet Explorer to run.

## License
This script is provided under the [MIT License](LICENSE).

