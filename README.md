# SpawnProtection
Documentation for the plugin SpawnProtection

Lightweight, reliable and modern spawn protection for Paper servers.

SpawnProtection protects your server spawn area against griefing, PvP, explosions, fluid abuse, piston exploits, entity manipulation and many other common forms of disruption.

Designed for server owners who want a simple, fast and dependable solution without WorldGuard, complicated regions or unnecessary dependencies.

---

## Features

### Spawn Area Protection

Protect your spawn using:

* Radius mode (cylindrical or spherical)
* Full-world protection mode
* Custom spawn center
* Automatic world spawn fallback

### Building Protection

Prevent players from:

* Breaking blocks
* Placing blocks
* Interacting with protected containers and mechanisms
* Trampling farmland
* Triggering pressure plates

### PvP Protection

Keep your spawn safe from combat:

* Blocks melee attacks
* Blocks projectile attacks
* Prevents attacks involving players inside the protected area
* Supports bypass permissions

### Explosion Protection

Protect the spawn from:

* TNT
* Creepers
* Beds and anchors
* Other entity and block explosions

### Fluid Protection

Prevents:

* Water placement
* Lava placement
* Bucket filling inside protected areas
* Fluid flow into protected areas

### Piston Protection

Stops piston-based bypasses:

* Moving blocks into protected areas
* Moving blocks out of protected areas
* Extending piston heads into protected areas
* Sticky piston exploits

### Entity Protection

Protects decorative and passive entities:

* Armor Stands
* Item Frames
* Glow Item Frames
* Paintings
* Villagers
* Animals
* Boats
* Minecarts
* End Crystals
* Other decorative entities

Players cannot damage, manipulate or remove protected entities inside the spawn area.

### Dispenser Protection

Blocks dispensers and droppers from placing or launching protected objects into the spawn area, including:

* Water and lava buckets
* Spawn eggs
* Armor stands
* Item frames
* Paintings
* Boats
* Minecarts
* TNT
* Fire charges
* End crystals

### Admin Tools

* Spawn preview particles
* Live configuration reload
* Custom spawn center commands
* Configuration migration system
* Automatic backup creation during migrations

### Multi-Language Support

Built-in translations:

* English
* Spanish
* Portuguese (Brazil)

---

## Commands

| Command            | Description                                 |
| ------------------ | ------------------------------------------- |
| `/spl help`        | Show available commands                     |
| `/spl info`        | Display current protection information      |
| `/spl reload`      | Reload configuration files                  |
| `/spl preview`     | Preview the protected area with particles   |
| `/spl setcenter`   | Set a custom spawn center                   |
| `/spl resetcenter` | Reset the custom center and use world spawn |

---

## Permissions

| Permission                  | Description                 |
| --------------------------- | --------------------------- |
| `spawnprotection.admin`     | Full administrative access  |
| `spawnprotection.reload`    | Reload configuration        |
| `spawnprotection.info`      | View protection information |
| `spawnprotection.preview`   | Preview protected area      |
| `spawnprotection.setcenter` | Set or reset spawn center   |
| `spawnprotection.bypass`    | Bypass all protections      |

---

## Installation

1. Download the latest release.
2. Place the plugin in your server's `plugins` folder.
3. Restart the server.
4. Edit the configuration if desired.
5. Use `/spl reload` after making changes.

---

## Configuration

Example:

```yaml
spawn:
  mode: radius
  radius: 20
  shape: cylinder

protections:
  block-break: true
  block-place: true
  pvp: true
  explosions: true
  fluids: true
  pistons: true
  entities: true
```

### Protection Modes

#### Radius Mode

Protects a configurable area around the spawn center.

```yaml
spawn:
  mode: radius
```

#### World Mode

Protects the entire world.

```yaml
spawn:
  mode: world
```

---

## Why SpawnProtection?

Many protection plugins are powerful but often excessive for simple servers.

SpawnProtection focuses on one job:

**Keeping your spawn safe.**

No regions.

No dependencies.

No unnecessary complexity.

Just lightweight and reliable spawn protection.

---

## Compatibility

* Paper
* Purpur
* Compatible Paper forks

Minecraft:

* 1.20.6
* 1.21.x
* 26.1 - 26.2

---

## Performance

SpawnProtection is designed to be lightweight and efficient.

* No databases
* No dependencies
* Minimal memory usage
* Event-driven architecture
* Suitable for both small and large servers

---
