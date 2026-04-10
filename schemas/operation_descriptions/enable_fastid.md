**Description:**
Enables FastID feature so tags return both EPC (Electronic Product Code) and TID (Tag Identifier) in a single inventory response.

**Usage:**
Send this command to activate FastID on the reader. Once enabled, each tag inventory response includes both the EPC and TID simultaneously, eliminating the need for separate TID read operations. This significantly improves inventory throughput and reduces the number of RF transmissions required.

**Persistence:** FastID remains active across stop/start cycles as long as the MQTT session stays connected. A reader reboot or MQTT disconnect clears the setting, and you must re-send this command to re-enable it.

**Parameters:**
- `enabled` (boolean): Set to `true` to enable FastID feature