**Radio Control Commands**

Use the radio control commands to start and stop the reader. You must stop the radio before applying Gen2X configuration changes, then restart it with `applyImpinjGen2X` set to `true` for the settings to take effect.

**Key Features:**
- **Synchronized Control**: Stop-configure-start workflow prevents configuration conflicts
- **State Management**: Proper sequencing ensures clean configuration application
- **Feature Activation**: Gen2X settings only activate on start with flag enabled
- **Clean Shutdown**: Stops all RF transmissions and inventory operations

**Configuration Workflow:**
1. Send `stop` command to halt radio and RF operations
2. Configure Gen2X settings (Protection, FastID, TagFocus, Quieting, etc.)
3. Send `start_with_gen2x` command with `applyImpinjGen2X` set to `true`
4. All configured features become active

**Related Commands:**
- `stop`: Halt radio and all RF transmissions
- `start_with_gen2x`: Start radio with Gen2X configurations applied
- `get_gen2x_config`: Verify current configuration before starting

**Important Requirements:**
- Configuration changes REQUIRE stopping the radio first
- Set `applyImpinjGen2X` to `true` for features to activate
- Always wait for success response before proceeding
- Atomicity: Stop, configure, then start as coordinated sequence

**Use Cases:**
- **Configuration Management**: Apply multiple settings in coordinated manner
- **Feature Activation**: Enable FastID, TagFocus, TagProtect, Tag Quieting
- **State Reset**: Stop and restart to clear session state
- **Maintenance**: Halt operations for system checks or updates
