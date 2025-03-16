# Multiloader Templates with Deimos  

This is a template for the [Minecraft Development IntelliJ Plugin](https://plugins.jetbrains.com/plugin/8327-minecraft-development), based on the built-in MultiLoader template. MultiLoader allows you to develop Minecraft mods for multiple loaders within a single environment. You can learn more about it [here](https://github.com/jaredlll08/MultiLoader-Template).  

I created this template to speed up my own Minecraft mod development, but feel free to download and customize it for your own projects.  

## Advantages Over the Built-in Template  

- **Two Template Options:**  
  - `multiloader` for Minecraft 1.21.1, based on the default 1.21 template (intended for 1.21+)
  - `oldmultiloader` for Minecraft 1.20.4, designed for older versions with support for only Fabric and Forge (intended for 1.18-1.20.4)

- **Mod Menu Dependency:**  
  Includes [Mod Menu](https://modrinth.com/mod/modmenu), a Fabric mod that lets you view and configure your mods in-game, as a preconfigured dependency

- **Deimos Dependency:**  
  Includes [Deimos](https://github.com/Mars-The-Planet/Deimos), a configuration and dynamic recipe generation library, as a preconfigured dependency

- **Cleaner Code:**  
  No debug prints, generic comments, or default loader-specific mixins

- **Additional Configuration:**  
  Added a `homepage` option in `gradle.properties`

## How to set it up
You can set it up easily in IntelliJ by adding a remote repository in Minecraft Development Settings. Follow these steps:  
1. Go to `File > Settings > Languages & Frameworks > Minecraft Development`
2. Add a remote repository  
3. Set the **Download URL** to:  
   `https://github.com/Mars-The-Planet/Multiloader-Templates-with-Deimos/archive/refs/heads/v1.zip`  

![Minecraft Development Settings](https://i.imgur.com/o0iyQiz.png)  

## How to change Minecraft versions

For 1.20.6 and onwards, use `multiloader`; for 1.18 to 1.20.4, use `oldmultiloader`. To change Minecraft versions, you will need to edit `gradle.properties` values like this:
### For 1.21.4
**Note:** You’ll also need to change `data()` to `clientData()` in `build.gradle (:neoforge)`.  
```
minecraft_version=1.21.4
modmenu_version=13.0.0-beta.1
minecraft_version_range=[1.21.4, 1.22)
neo_form_version=1.21.4-20241203.161809
parchment_minecraft=1.21.4
parchment_version=2024.12.22
# Fabric
fabric_version=0.112.2+1.21.4
fabric_loader_version=0.16.9
# Forge
forge_version=54.0.10
forge_loader_version_range=[54,)
# NeoForge
neoforge_version=21.4.33-beta
neoforge_loader_version_range=[4,)
```
### For 1.21.3
```
minecraft_version=1.21.3
modmenu_version=12.0.0
minecraft_version_range=[1.21.2, 1.22)
neo_form_version=1.21.3-20241023.131943
parchment_minecraft=1.21
parchment_version=2024.11.10
# Fabric
fabric_version=0.109.0+1.21.3
fabric_loader_version=0.16.9
# Forge
forge_version=53.0.21
forge_loader_version_range=[53,)
# NeoForge
neoforge_version=21.3.36-beta
neoforge_loader_version_range=[4,)
```
### For 1.21-1.21.1
**Note:** This is what the mod will be set to if you use the `multiloader` template
```
minecraft_version=1.21.1
modmenu_version=11.0.3
minecraft_version_range=[1.21, 1.22)
neo_form_version=1.21.1-20240808.144430
parchment_minecraft=1.21
parchment_version=2024.11.10
# Fabric
fabric_version=0.109.0+1.21.1
fabric_loader_version=0.16.9
# Forge
forge_version=52.0.28
forge_loader_version_range=[51,)
# NeoForge
neoforge_version=21.1.80
neoforge_loader_version_range=[4,)
```
### For 1.20.5-1.20.6
```
minecraft_version=1.20.6
modmenu_version=10.0.0
minecraft_version_range=[1.20.5, 1.21)
neo_form_version=1.20.6-20240627.102356
parchment_minecraft=1.20.6
parchment_version=2024.06.16
# Fabric
fabric_version=0.100.8+1.20.6
fabric_loader_version=0.16.9
# Forge
forge_version=50.1.0
forge_loader_version_range=[50,)
# NeoForge
neoforge_version=20.6.122
neoforge_loader_version_range=[2,)
```
### For 1.20.3-1.20.4
**Note:** This is what the mod will be set to if you use the `oldmultiloader` template
```
minecraft_version=1.20.4
minecraft_version_range=[1.20.3, 1.21)
modmenu_version=9.0.0
# Fabric
fabric_version=0.97.2+1.20.4
fabric_loader_version=0.16.9
# Forge
forge_version=49.0.19
forge_loader_version_range=[49,)
```
### For 1.20.2
```
minecraft_version=1.20.2
modmenu_version=8.0.1
minecraft_version_range=[1.20.2, 1.21)
# Fabric
fabric_version=0.91.6+1.20.2
fabric_loader_version=0.16.9
# Forge
forge_version=48.0.49
forge_loader_version_range=[48,)
```
### For 1.20-1.20.1
```
minecraft_version=1.20.1
modmenu_version=7.2.2
minecraft_version_range=[1.20, 1.21)
# Fabric
fabric_version=0.92.2+1.20.1
fabric_loader_version=0.16.9
# Forge
forge_version=47.2.30
forge_loader_version_range=[46,)
```
### For 1.19.4
```
minecraft_version=1.19.4
modmenu_version=6.3.1
minecraft_version_range=[1.19.4, 1.20)
# Fabric
fabric_version=0.87.2+1.19.4
fabric_loader_version=0.16.9
# Forge
forge_version=45.3.15
forge_loader_version_range=[45,)
```
### For 1.19-1.19.2
```
minecraft_version=1.19.2
modmenu_version=4.2.0-beta.2
minecraft_version_range=[1.19, 1.20)
# Fabric
fabric_version=0.77.0+1.19.2
fabric_loader_version=0.16.9
# Forge
forge_version=43.4.12
forge_loader_version_range=[41,)
```
### For 1.18 - 1.18.2
```
minecraft_version=1.18.2
modmenu_version=3.2.5
minecraft_version_range=[1.18, 1.19)
# Fabric
fabric_version=0.77.0+1.18.2
fabric_loader_version=0.16.9
# Forge
forge_version=40.3.0
forge_loader_version_range=[38,)
```
