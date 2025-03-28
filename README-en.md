# NCHUIT-MCServer
*Check out README in different languages: [繁體中文](README.md)*

## 📋 Introduction
This is the official Minecraft server of NCHUIT (National Chung Hsing University Information Technology Club)!

This is a modded server, and we use [Manual-MMDM](https://github.com/coke5151/manual-mmdm) to manage and export client/server mods separately.

## 🎮 Game Information
- **Game Version**: `1.19.2`
- **Mod Loader**: `Forge`
- **Forge Version**: `1.19.2-43.4.0`
- **Server Address**: `nchuit.ddns.net`
- **Memory Requirement**: We recommend allocating at least 4GB RAM to the game.

## 📊 Mod List and Dependencies
You can find a complete list of all mods and their dependencies in the [dependency-tree.txt](./manual-mmdm/dependency-tree.txt) file. This file is automatically generated using the Manual-MMDM tool and provides detailed information about:
- All mods included in the server
- Version information for each mod
- Dependencies between different mods

## ⚙️ Mod Features
- This server includes a variety of mods that enhance game experience
- Balanced gameplay and social interaction features
- Regular updates and maintenance
- The server uses CraftTweaker to remove some crafting recipes for better game balance
- Some mods have been manually translated to Chinese, so the files may differ from those downloaded from CurseForge

## 📥 Client Setup
> 💡 **Installation guide with images** available at [HackMD](https://hackmd.io/@113team/S1zUeqdQyg)

> ⚠️ **Note**: When first launching the game after installing the modpack, you will see a welcome page from the MTR mod. Please follow the on-screen instructions and wait patiently for about 18 seconds before pressing ESC to close the welcome page.

### System Requirements
- **1.19.2 requires Java 17 or newer**

### Installation Methods
#### Using Prism Launcher (Recommended):
1. Download the `.zip` file that starts with Prism-Launcher from the Release section
2. Import the **zip file directly** into Prism Launcher (no need to extract)
3. Configure RAM and Java settings

#### Manual Installation (Official Launcher):
1. Install the specified Forge version
2. Download the `.zip` file that starts with Client-Mods from the Release section
3. Extract and place the mods into the `.minecraft/mods` folder
4. Configure your Minecraft launcher to ensure it's running the Forge version and allocate at least 3GB memory

## 🖥️ Server Setup
- We recommend using the newer [Adoptium distribution](https://adoptium.net/) instead of OpenJDK

### Steps
1. Download the `.zip` file that starts with Server-Template and extract it
2. Edit `user_jvm_args.txt` to set the RAM allocation, recommended at least 6GB
3. On Windows run `run.bat` / On Linux run `run.sh` to start the server!

> ⚠️ **Note**: On first run, an `eula.txt` file will be generated. Remember to edit this file to agree to the terms before restarting the server! (This step is the same as all Minecraft server setup processes; you can search for tutorials online)

> ⚠️ **Warning**: The server has an automatic restart feature. If you don't properly set the `eula=true` in eula.txt after the first run, the server might get stuck in a restart loop. Make sure to edit the file between restarts!

## 🔧 Mod Management
Download the latest version of [Manual-MMDM](https://github.com/coke5151/manual-mmdm), place it in the manual-mmdm folder, and make sure all managed mods are placed in `manual-mmdm/mods`.

> ⚠️ **Important**: Always remember to use the "Export JSON" and "Generate Dependency Tree" functions in the Manual-MMDM tool before committing any changes to the repository. This ensures that all mod dependencies are properly documented and tracked. It is recommended to place the generated dependency-tree file in the project root directory and the manual-mmdm.json file in the manual-mmdm folder.

## 📦 Publishing Guide
If you're a modpack editor and want to publish a Release after changing mods, prepare the following files:

1. `Client-Mods-<tag>.zip`: Contains all client-side mods exported using [Manual-MMDM](https://github.com/coke5151/manual-mmdm)
2. `Prism-Launcher-<tag>.zip`: Place the client mods exported from Manual-MMDM into the Repository's `prism-launcher-template/minecraft/mods` folder, then compress the entire `prism-launcher-template` folder and rename it
3. `Server-Template-<tag>.zip`: Download the server template from this Repository's `server-template` folder, place the server mods exported from Manual-MMDM into `server-template/mods`. This zip file when extracted should include the entire server template + mods.

**Pre-commit Checklist**:
- Use the "Export JSON" function in Manual-MMDM to update mod information
- Use the "Generate Dependency Tree" function to document mod dependencies
- Verify all changes are properly documented before committing

## ❓ Frequently Asked Questions (FAQ)
1. **Issue**: Memory error when launching the game  
   **Solution**: Make sure you've allocated enough RAM to Minecraft (at least 4GB)

2. **Issue**: Unable to connect to the server  
   **Solution**: Verify that the server address is entered correctly and check your network connection

3. **Issue**: Mods showing as version incompatible  
   **Solution**: Ensure you're using the correct Forge and Minecraft versions (1.19.2 and Forge 1.19.2-43.4.0)

## 📞 Contact Us
If you have any questions or suggestions, feel free to contact us through:
- Email: [it.nchu@gmail.com](mailto:it.nchu@gmail.com)
- Club Website: [nchuit.com](https://nchuit.com/)

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
