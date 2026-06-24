# FAQ

Frequently Asked Questions about SpawnProtection.

---

# Does SpawnProtection require WorldGuard?

No.

SpawnProtection is a standalone plugin and does not require WorldGuard or any other protection plugin.

Simply install the plugin and start using it.

---

# Can I protect an entire world?

Yes.

Set the protection mode to:

```yaml
spawn:
  mode: world
```

This will protect the entire configured world instead of a radius around spawn.

---

# Can I use a custom spawn center?

Yes.

The easiest way is:

```text
/spl setcenter
```

This will set the protection center to your current location.

To return to the world's spawn location:

```text
/spl resetcenter
```

---

# Can administrators bypass protection?

Yes.

Players with:

```text
spawnprotection.bypass
```

can bypass all protection checks.

This permission is intended for administrators and trusted staff.

---

# Does SpawnProtection protect against PvP?

Yes.

When PvP protection is enabled:

```yaml
protections:
  pvp: true
```

players cannot attack each other inside the protected area.

Both melee and projectile attacks are supported.

---

# Does SpawnProtection protect against TNT and Creepers?

Yes.

Explosion protection covers:

* TNT
* Creepers
* Beds
* Respawn Anchors
* Other explosion sources

Example:

```yaml
protections:
  explosions: true
```

---

# Does SpawnProtection protect against water and lava griefing?

Yes.

Fluid protection includes:

* Water bucket placement
* Lava bucket placement
* Bucket filling
* Water flow
* Lava flow

Example:

```yaml
protections:
  fluids: true
```

---

# Does SpawnProtection protect against piston exploits?

Yes.

When piston protection is enabled:

```yaml
protections:
  pistons: true
```

the plugin prevents:

* Moving blocks into protected areas
* Moving blocks out of protected areas
* Sticky piston exploits
* Piston extension into protected areas

---

# Does SpawnProtection protect Armor Stands and Item Frames?

Yes.

Entity protection includes:

* Armor Stands
* Item Frames
* Glow Item Frames
* Paintings
* Villagers
* Animals
* Boats
* Minecarts
* End Crystals

Example:

```yaml
protections:
  entities: true
```

---

# Can players interact with chests inside spawn?

No, if block placement/interactions protection is enabled.

SpawnProtection blocks interaction with many common containers and mechanisms, including:

* Chests
* Barrels
* Furnaces
* Hoppers
* Doors
* Trapdoors
* Levers
* Buttons
* Pressure Plates

---

# Is SpawnProtection compatible with Paper?

Yes.

SpawnProtection is designed primarily for:

* Paper
* Purpur
* Most Paper forks

---

# Which Minecraft versions are supported?

Current releases support:

```text
Minecraft 1.20.6+
```

including modern 1.21.x versions.
26.1 - 26.2

Always check the latest release notes for updated compatibility information.

---

# Does SpawnProtection support multi-language messages?

Yes.

Built-in languages include:

* English
* Spanish
* Portuguese (Brazil)

Example:

```yaml
settings:
  language: es
```

---

# Can I reload the configuration without restarting?

Yes.

Use:

```text
/spl reload
```

to reload the configuration and message files.

A full server restart is not required.

---

# Will updates overwrite my configuration?

No.

SpawnProtection includes an automatic configuration migration system.

When possible:

* Existing values are preserved
* Missing settings are added automatically
* Backups are created before migrations

---

# Is SpawnProtection lightweight?

Yes.

The plugin was designed to be lightweight and efficient.

Features include:

* No database
* No dependencies
* Minimal memory usage
* Event-driven architecture
* Suitable for both small and large servers

---

# Why use SpawnProtection instead of a region plugin?

Region plugins are powerful, but many servers only need one thing:

A protected spawn.

SpawnProtection focuses exclusively on spawn protection and provides a simpler setup, lower overhead and fewer configuration requirements than full region-management solutions.

---

# I found a bug. What should I do?

Please open an issue and include:

* Minecraft version
* Server software (Paper, Purpur, etc.)
* SpawnProtection version
* Steps to reproduce the issue
* Any relevant console errors

The more information provided, the easier it is to investigate and resolve the problem.
