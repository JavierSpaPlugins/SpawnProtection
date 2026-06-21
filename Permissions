# Permissions

This page documents all permissions available in SpawnProtection.

---

# Overview

SpawnProtection uses a simple permission structure designed for administrators and staff.

Most servers only need:

```text id="rn0v2o"
spawnprotection.admin
```

which grants access to all administrative commands.

---

# Permission List

| Permission                  | Description                           | Default |
| --------------------------- | ------------------------------------- | ------- |
| `spawnprotection.admin`     | Full administrative access            | OP      |
| `spawnprotection.reload`    | Reload plugin configuration           | OP      |
| `spawnprotection.info`      | View protection information           | OP      |
| `spawnprotection.preview`   | Preview protected area with particles | OP      |
| `spawnprotection.setcenter` | Set or reset the protection center    | OP      |
| `spawnprotection.bypass`    | Bypass all spawn protection checks    | OP      |

---

# Permission Details

## spawnprotection.admin

```text
spawnprotection.admin
```

Grants access to all administrative features.

Includes:

* Reload configuration
* View protection information
* Preview protected area
* Set custom spawn center
* Reset custom spawn center

Recommended for:

* Server Owners
* Administrators

---

## spawnprotection.reload

```text
spawnprotection.reload
```

Allows use of:

```text
/spl reload
```

Recommended for:

* Administrators
* Senior Staff

---

## spawnprotection.info

```text
spawnprotection.info
```

Allows use of:

```text
/spl info
/spl help
```

Recommended for:

* Administrators
* Moderators
* Staff Members

---

## spawnprotection.preview

```text
spawnprotection.preview
```

Allows use of:

```text
/spl preview
```

Displays temporary particles showing the protected area boundaries.

Recommended for:

* Administrators
* Builders
* Spawn Designers

---

## spawnprotection.setcenter

```text
spawnprotection.setcenter
```

Allows use of:

```text
/spl setcenter
/spl resetcenter
```

Recommended for:

* Administrators
* Server Owners

---

## spawnprotection.bypass

```text
spawnprotection.bypass
```

Bypasses all protection checks.

Players with this permission can:

* Break protected blocks
* Place protected blocks
* Interact with protected containers
* Bypass PvP protection
* Bypass fluid restrictions
* Bypass entity protection
* Bypass piston-related restrictions

Recommended for:

* Administrators only

Be careful when assigning this permission to regular staff members.

---

# Permission Examples

## LuckPerms

Grant full administrative access:

```text
/lp user Steve permission set spawnprotection.admin true
```

Grant bypass access:

```text
/lp user Steve permission set spawnprotection.bypass true
```

Grant preview access only:

```text
/lp user Builder permission set spawnprotection.preview true
```

---

# Recommended Setup

## Owner

```text
spawnprotection.admin
spawnprotection.bypass
```

---

## Administrator

```text
spawnprotection.admin
```

---

## Builder

```text
spawnprotection.preview
spawnprotection.info
```

---

## Moderator

```text
spawnprotection.info
```

---

# Notes

* All permissions are compatible with common permission plugins such as LuckPerms.
* Server operators (OPs) have access by default.
* The bypass permission should be granted carefully, as it disables all protection checks for the player.
