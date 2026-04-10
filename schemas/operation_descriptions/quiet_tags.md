**Description:**
Selectively silences one or more specific tags by their EPC ID, preventing them from responding to inventory rounds without affecting other tags.

**Usage:**
Send this command with an array of one or more EPC IDs to quiet. Quieted tags will not participate in inventory responses and will not transmit RF signals to the reader. This is useful for isolating problematic tags, managing high-density inventory operations, or testing specific tag subsets. You can quiet up to 31 tag EPCs in a single command.

**Persistence:** Quieted tags remain silent across stop/start cycles as long as the MQTT session stays connected. A reader reboot or MQTT disconnect clears the quiet state, and you must re-send this command to re-quiet them. Use the Unquiet Tags command to explicitly restore individual tags.

**Parameters:**
- `action` (string): Set to `quiet` to silence tags
- `tagIDs` (array): List of one or more EPC IDs as strings to silence
  - Minimum 1 tag required
  - Format: EPC ID strings matching tag identifier format

