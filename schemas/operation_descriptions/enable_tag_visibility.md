**Description:**
Grants the reader temporary authorization to see and read protected tags by providing the correct 32-bit access password.

**Usage:**
Send this command with the 32-bit access password. The reader will use this password to authenticate and unmask all protected tags that match this password during inventory rounds. This allows the reader to interact with protected tags without permanently unlocking them.

**Persistence:** The authorization remains active across stop/start cycles as long as the MQTT session stays connected. A reader reboot or MQTT disconnect clears the authorization, and you must re-send this command to restore visibility.

**Parameters:**
- `action` (string): Set to `enableTagVisibility` to allow inventory of protected tags
- `password` (string): A 32-bit (8-character hexadecimal) access password for authentication
