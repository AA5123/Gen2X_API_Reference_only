## stop

**Description:**
Stops the reader radio immediately, halting all inventory operations and RF transmissions.

**Usage:**
Send this command with an empty payload to stop the reader radio. You must stop the radio before applying any Gen2X configuration changes such as enabling/disabling tag protection, FastID, TagFocus, or tag quieting. Always wait for the success response before attempting to configure settings or restart the radio. Stopping the reader is mandatory for synchronized configuration management.

**Parameters:**
- None (empty payload required)

**Behavior:**
- Radio stops immediately
- All inventory operations cease
- RF transmissions halt
- Reader enters idle state
- Must stop before applying Gen2X configurations
- Configuration changes only take effect on next `start_with_gen2x` command
