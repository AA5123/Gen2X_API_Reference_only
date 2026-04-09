## enable_tag_visibility

**Description:**
Grants the reader temporary authorization to see and read protected tags by providing the correct 32-bit access password.

**Usage:**
Send this command with the 32-bit access password. The reader will use this password to authenticate and unmask all protected tags that match this password during inventory rounds. This allows the reader to interact with protected tags without permanently unlocking them. The authorization persists until you use `disable_tag_visibility` or disconnect.

**Parameters:**
- `password` (string): A 32-bit (8-character hexadecimal) access password for authentication

**Behavior:**
- Reader authenticates with protected tags using the provided password
- Protected tags become visible in inventory results
- Tag remains in protected state (not unlocked)
- All tags matching this password become readable
- Authorization is session-based and persistent until disabled
