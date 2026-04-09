## disable_fastid

**Description:**
Disables the FastID feature, returning tags to standard inventory mode where they return only the EPC (Electronic Product Code).

**Usage:**
Send this command to deactivate FastID on the reader. Once disabled, tags will only return their EPC in inventory responses. If you need the TID (Tag Identifier), you must perform a separate dedicated TID read operation. This is useful for reducing response payload size or simplifying data processing when TID data is not required.

**Parameters:**
- `enabled` (boolean): Set to `false` to disable FastID feature

**Behavior:**
- Tags return only EPC in inventory responses
- TID is no longer included in standard inventory
- Separate TID read operations required if TID data needed
- Response payload size decreases
- Feature remains disabled across reader sessions until re-enabled
