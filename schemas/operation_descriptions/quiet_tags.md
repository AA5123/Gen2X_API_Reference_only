## quiet_tags

**Description:**
Selectively silences one or more specific tags by their EPC ID, preventing them from responding to inventory rounds without affecting other tags.

**Usage:**
Send this command with an array of one or more EPC IDs to quiet. Quieted tags will not participate in inventory responses and will not transmit RF signals to the reader. This is useful for isolating problematic tags, managing high-density inventory operations, or testing specific tag subsets. Quieted tags remain silent until explicitly restored with `unquiet_tags`. You can quiet up to the maximum number of tags supported by your reader configuration.

**Parameters:**
- `action` (string): Set to `quiet` to silence tags
- `tagIDs` (array): List of one or more EPC IDs as strings to silence
  - Minimum 1 tag required
  - Format: EPC ID strings matching tag identifier format

**Behavior:**
- Specified tags stop responding to inventory operations
- Quieted tags do not transmit RF signals
- Other tags continue normal inventory participation
- Quiet state persists until explicitly unquieted
- Multiple quiet commands accumulate tag silence list
