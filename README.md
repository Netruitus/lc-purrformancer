# Lethal Company - Purrformancer

## Compatible with v56

A modpack designed to improve gameplay performance and fix known bugs or inconvenience issues. It utilizes mods that are made for this purpose, tested together in normal and fully modded games. The aim of this modpack is to keep it simple and serve as a base for other modpacks or mod profiles. Updates will be provided as soon as possible to enhance the modding experience for the entire community.

## IMPORTANT NOTE

If you use any mods that is modifying masked enemies (like Skinwalkers or Mirage), you might want to disable fixes for them in config file `butterystancakes.lethalcompany.enemysoundfixes.cfg` - just change `FixMasks` to `false`.

## Applied Modifications

### **BepInEx**

By default, logging is disabled in this modpack. Logging primarily serves debugging purposes during mod or modpack development. For end-user products, logging should be disabled to conserve CPU resources, optimizing the game's performance.

### **StarlancerAIFix** by [AudioKnight](https://thunderstore.io/c/lethal-company/p/AudioKnight)

Dynamically assigns appropriate AI behaviors to enemies upon spawning, based on their location within or outside dungeons. Additionally, it resolves a null reference exception related to EnableEnemyMesh().

### **FixRPCLag** by [Bobbie](https://thunderstore.io/c/lethal-company/p/Bobbie)

Addresses performance issues stemming from NetworkManager.LogLevel set to Developer, which triggers significant lag spikes due to printing RPC Table Contents for every RPC error. To mitigate this, we have fully disabled logging levels, ensuring smoother gameplay without interruptions caused by excessive logging.

### **EnemySoundFixes** by [ButteryStancakes](https://thunderstore.io/c/lethal-company/p/ButteryStancakes)

Addresses and fixes various sound issues in Lethal Company, enhancing the audio experience by correcting looping, missing sounds, and improperly pitched effects for different entities in the game. It ensures smoother and more immersive gameplay by resolving these audio problems.

### **NoJumpDelay** by [DaXcess](https://thunderstore.io/c/lethal-company/p/DaXcess)

Patches out the jump delay.

### **MoreItems** by [Drakorle](https://thunderstore.io/c/lethal-company/p/Drakorle)

Allows game saves with over 45 items, with support extended up to 999 items. No longer will items despawn upon saving, making it especially handy when combined with mods supporting more than 4 players or when strategically spending credits on items to evade the on-death penalty. However, caution is advised against overloading your system with an excessive number of items, as it may strain your computer's performance.

### **CleanerLogs** by [EliteMasterEric](https://thunderstore.io/c/lethal-company/p/EliteMasterEric)

An additional layer to streamline logging processes, this mod comes pre-configured to set log levels to Exceptions only. Ideal for instances where other mods interfere with logging, it efficiently minimizes unnecessary log messages, providing a performance boost for systems with limited processing power.

### **FixPluginTypesSerialization** by [Evaisa](https://thunderstore.io/c/lethal-company/p/Evaisa)

Integrates with the native Unity engine to include BepInEx plugin assemblies in the assembly list, typically reserved for assemblies within the game's Managed/ folder. This resolves a critical bug where custom Serializable structs and similar elements stored in plugin assemblies fail to deserialize properly within the engine.

### **LetMeLookDown** by [FlipMods](https://thunderstore.io/c/lethal-company/p/FlipMods)

Allows you to nearly fully look downward in-game, enhancing your perspective and immersion.

### **CullFactory** by [fumiko](https://thunderstore.io/c/lethal-company/p/fumiko)

Optimizes rendering by culling objects not in view or too distant from the camera, enhancing performance. It's compatible with mods adding cameras, offering two culling methods:

- **Portal Occlusion Culling**: Hides non-visible objects without affecting visuals, enhancing immersion.
- **Depth Culling**: Renders objects within a certain distance from the camera, prioritizing performance.

### **LCMaxSoundsFix** by [Hardy](https://thunderstore.io/c/lethal-company/p/Hardy)

Boosts the maximum number of simultaneously playing sounds in the Unity engine. It should fix for example missing footsteps or sounds issue in Lethal Company, especially prevalent in modded versions.

### **DoorFix** by [itsmeowdev](https://thunderstore.io/c/lethal-company/p/itsmeowdev)

Corrects door hitboxes, facilitating easier item pickups through open doors. However, it requires aiming at the door to close it, which may be seen as both a benefit and a drawback.

### **DissonanceLagFix** by [linkoid](https://thunderstore.io/c/lethal-company/p/linkoid)

An additional layers to reduce lag spike durations by adjusting the log level of DissonanceVoip. By addressing the issue where DissonanceVoip spamming warnings during lag spikes prolongs the duration, this plugin cuts lag spike durations in half by limiting logging to errors only.

### **AsyncLoggers** by [mattymatty](https://thunderstore.io/c/lethal-company/p/mattymatty)

An additional layer that moves each logging operation to its own thread, separating it from in-game operations and eliminating delays caused by logging. The impact of this improvement grows with the volume of logs generated by your modpack, making it a crucial addition for smoother gameplay.

### **PathfindingLagFix** by [Zaggy1024](https://thunderstore.io/c/lethal-company/p/Zaggy1024)

Optimizes the AI behavior of Bracken, Snare Flea, and Spore Lizard to prevent performance stutters that can occur every 200 milliseconds in specific situations. By distributing the workload of path checks over multiple frames, it mitigates issues stemming from excessive node accessibility checks, improving overall gameplay stability.

## Support

All suggestions and feedback are welcome, particularly from mod developers (I'm open for a cooperation). Join my Discord at https://discord.gg/hTuqEUmeg3 to share your thoughts and ideas!
