**Description:**
Stops the reader radio immediately, halting all inventory operations and RF transmissions.

**Usage:**
Send this command with an empty payload to stop the reader radio. You must stop the radio before applying any Gen2X configuration changes such as enabling/disabling tag protection, FastID, TagFocus, or tag quieting. Always wait for the success response before attempting to configure settings or restart the radio. Stopping the reader is mandatory for synchronized configuration management.

**Parameters:**
- None (empty payload required)

**Behavior:**
- Radio and RF inventory activity stop immediately
- Reader enters idle state for safe configuration changes
- New Gen2X settings apply on the next start with Gen2X enabled
