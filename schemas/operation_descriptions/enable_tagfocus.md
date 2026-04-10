**Description:**
Enables TagFocus feature so tags that have already been inventoried remain silent in subsequent inventory rounds, allowing the reader to focus exclusively on new or unread tags.

**Usage:**
Send this command to activate TagFocus on the reader. Once enabled, any tag that has been successfully read in the current session (S1) will stop responding to subsequent inventory rounds. This dramatically improves read rates in dense tag environments by eliminating duplicate reads and concentrating RF energy on newly encountered tags.

**Persistence:** TagFocus remains active across stop/start cycles as long as the MQTT session stays connected. A reader reboot or MQTT disconnect clears the setting, and you must re-send this command to re-enable it.

**Parameters:**
- `enabled` (boolean): Set to `true` to enable TagFocus feature
