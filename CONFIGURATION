# Configuration

SpawnProtection is designed to work out of the box with minimal setup, but every protection feature can be configured individually.

After editing the configuration, use:

```text
/spl reload
```

or restart the server.

---

# Spawn Settings

## Protection Mode

```yaml
spawn:
  mode: radius
```

Available values:

| Value    | Description                                         |
| -------- | --------------------------------------------------- |
| `radius` | Protect a configurable area around the spawn center |
| `world`  | Protect the entire world                            |

### Radius Mode

Example:

```yaml
spawn:
  mode: radius
  radius: 20
```

Players are protected inside the configured radius.

### World Mode

Example:

```yaml
spawn:
  mode: world
```

The entire world becomes protected.

---

## Radius

```yaml
spawn:
  radius: 20
```

Defines the size of the protected area when using `radius` mode.

Default:

```yaml
radius: 20
```

---

## Shape

```yaml
spawn:
  shape: cylinder
```

Available values:

| Value      | Description                                               |
| ---------- | --------------------------------------------------------- |
| `cylinder` | Horizontal protection only (recommended for most servers) |
| `sphere`   | Full 3D spherical protection                              |

### Cylinder

Protects players within the configured X/Z radius regardless of height.

### Sphere

Protects players within a true spherical area.

---

# Custom Spawn Center

SpawnProtection can use either:

* The world's spawn location
* A custom center location

Example:

```yaml
spawn:
  custom-center:
    enabled: true
    world: world
    x: 100
    y: 64
    z: -50
```

The easiest way to configure this is:

```text
/spl setcenter
```

To return to the world's spawn:

```text
/spl resetcenter
```

---

# Protection Options

All protections can be enabled or disabled individually.

---

## Block Breaking

```yaml
protections:
  block-break: true
```

Prevents players from breaking blocks inside the protected area.

---

## Block Placement

```yaml
protections:
  block-place: true
```

Prevents players from placing blocks inside the protected area.

This also protects many common interactable blocks such as:

* Chests
* Barrels
* Furnaces
* Doors
* Trapdoors
* Levers
* Buttons
* Pressure Plates
* Repeaters
* Comparators

---

## PvP

```yaml
protections:
  pvp: true
```

Prevents combat inside the protected area.

Includes:

* Melee attacks
* Projectile attacks
* Crossbows
* Tridents

---

## Explosions

```yaml
protections:
  explosions: true
```

Protects the area from explosions.

Includes:

* TNT
* Creepers
* Beds
* Respawn Anchors
* Other explosion sources

---

## Fluids

```yaml
protections:
  fluids: true
```

Prevents fluid-related griefing.

Includes:

* Water bucket placement
* Lava bucket placement
* Bucket filling
* Water flow into protected areas
* Lava flow into protected areas

---

## Pistons

```yaml
protections:
  pistons: true
```

Prevents piston-based bypasses.

Includes:

* Pushing blocks into protected areas
* Pulling blocks out of protected areas
* Sticky piston exploits
* Piston head extension into protected areas

---

## Entities

```yaml
protections:
  entities: true
```

Protects decorative and passive entities inside the protected area.

Examples:

* Armor Stands
* Item Frames
* Glow Item Frames
* Paintings
* Villagers
* Animals
* Boats
* Minecarts
* End Crystals

Players cannot damage, manipulate or remove protected entities.

---

# Language

```yaml
settings:
  language: en
```

Available values:

| Value   | Language            |
| ------- | ------------------- |
| `en`    | English             |
| `es`    | Spanish             |
| `pt-br` | Portuguese (Brazil) |

Default:

```yaml
language: en
```

---

# Bypass Permission

Players with:

```text
spawnprotection.bypass
```

are not affected by protection checks.

This permission is intended for administrators and staff members.

---

# Configuration Migration

SpawnProtection includes an automatic migration system.

When a new version introduces configuration changes:

* Missing options are added automatically
* Existing values are preserved
* A backup of the previous configuration is created

This means most updates do not require deleting your configuration files.

---

# Recommended Configurations

## Small Survival Server

```yaml
spawn:
  mode: radius
  radius: 20
  shape: cylinder
```

Simple and lightweight protection around spawn.

---

## Large Hub Server

```yaml
spawn:
  mode: radius
  radius: 100
  shape: cylinder
```

Provides a large protected area for lobby environments.

---

## Fully Protected World

```yaml
spawn:
  mode: world
```

Protects the entire world from modifications.
