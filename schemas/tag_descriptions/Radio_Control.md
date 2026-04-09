Use the radio control commands to start and stop the reader. You must stop the radio before applying Gen2X configuration changes, then restart it with `applyImpinjGen2X` set to `true` for the settings to take effect.

**Key Features:**
- **Stop-Then-Configure Model**: Prevents applying settings while radio is active
- **Explicit Feature Activation**: `applyImpinjGen2X: true` applies staged settings on start
- **Operational Safety**: Clear transition between active and configuration states
