# Multiloader Templates with Deimos Dependency
This is a template for [Minecraft Development IntelliJ plugin](https://plugins.jetbrains.com/plugin/8327-minecraft-development). It is based on the built-in MultiLoader template. MultiLoader makes it possible to MC modsdevelop on multiple I made it to speed up the development of my Minecraft mods but feel free to download it and edit it. 
## Advantages over the built-in template
- Contains two templates:
  - one for 1.21.1, instead of 1.21 compared to the default template
  - and one for 1.20.4 with only Fabric and Forge for development on older MC versions
- Includes configuration and dynamic recipe generation library [Deimos](https://github.com/Mars-The-Planet/Deimos) as a dependency
- Has no debug prints, generic comments, or default loader-specific mixins
- in gradlew.properties added the option for the homepage
