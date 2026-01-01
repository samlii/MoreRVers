# MoreRVers - Multiplayer Expansion Mod for RV There Yet?

A runtime mod that increases the multiplayer player cap beyond the default 4-player limit for RV There Yet.

**Only the host needs to install the mod.**

## Overview

This mod patches the game's multiplayer cap at runtime, allowing you to host sessions with more than the default 4 players. The modification uses UE4SS for runtime patching without requiring binary editing or permanent game file changes.

## Features

- **Simple Configuration** - Single-value INI file configuration
- **Host-Only Requirement** - Clients do not require mod installation
- **Non-Destructive** - No permanent game file modifications
- **Flexible Limits** - Configurable player count from 1-24
- **Runtime Patching** - Applied immediately upon session creation

## Configuration

Edit `MoreRVers/config.ini`:

```ini
MaxPlayers = 8
```

**Configuration Parameters:**
- Default: 8 (vanilla game limit is 4)
- Range: 1-24
- Recommended: 8 for optimal stability

The game must be restarted for configuration changes to take effect.

## Verification

Successful installation can be verified by checking the UE4SS log for the following messages:

```
[MoreRVers] [INFO] MoreRVers v1.0.0 loading. Target cap=8 (hard max 24)
[MoreRVers] [INFO] Applied MaxPlayers override: 4 → 8
```

## Contributing

Bug reports and feature suggestions can be submitted via GitHub Issues. Pull requests are welcome.

## Credits

- **UE4SS Team** - Unreal Engine modding framework
- **RV There Yet? Community** - Testing and feedback
- **A-Zzi** - Original Author of Mod ([Original Project](https://github.com/a-zzi/morervers))