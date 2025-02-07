# Multiloader Templates with Deimos  

This is a template for the [Minecraft Development IntelliJ Plugin](https://plugins.jetbrains.com/plugin/8327-minecraft-development), based on the built-in MultiLoader template. MultiLoader allows you to develop Minecraft mods for multiple loaders within a single environment. You can learn more about it [here](https://github.com/jaredlll08/MultiLoader-Template).  

I created this template to speed up my own Minecraft mod development, but feel free to download and customize it for your own projects.  

## Advantages Over the Built-in Template  

- **Two Template Options:**  
  - One for Minecraft 1.21.1, updated from 1.21 in the default template  
  - One for Minecraft 1.20.4, designed for older versions with support for only Fabric and Forge  

- **Deimos Dependency:**  
  Includes [Deimos](https://github.com/Mars-The-Planet/Deimos), a configuration and dynamic recipe generation library, as a preconfigured dependency.  

- **Cleaner Code:**  
  No debug prints, generic comments, or default loader-specific mixins.  

- **Additional Configuration:**  
  Added a `homepage` option in `gradle.properties`.  

## How to set it up
You can easily set it up in Intellij by adding a remote repository in Minecraft Development Settings (you get there by going `File/Settings/Languages & Frameworks/Minecraft Development`) and setting its Download URL to `https://github.com/Mars-The-Planet/Multiloader-Templates-with-Deimos/archive/refs/heads/v1.zip`

![Minecraft Development Settings](https://i.imgur.com/o0iyQiz.png)

## How to change Minecraft versions

If you want to make a mod for 1.20.6 and further, or you just want to update a mod past 1.20.4 use the 1.21.1 template to create a new mod and then edit `gradle.properties` values like this:
### For 1.20.4
you also need to change data() to clientData() in `gradle.build (:neoforge)`
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
