## enable_fastid

**Description:**
Enables FastID feature so tags return both EPC (Electronic Product Code) and TID (Tag Identifier) in a single inventory response.

**Usage:**
Send this command to activate FastID on the reader. Once enabled, each tag inventory response includes both the EPC and TID simultaneously, eliminating the need for separate TID read operations. This significantly improves inventory throughput and reduces the number of RF transmissions required. FastID remains active until explicitly disabled.

**Parameters:**
- `enabled` (boolean): Set to `true` to enable FastID feature

**Behavior:**
- Tags return both EPC and TID in single response
- Inventory operations return dual data in one RF round
- Overall read throughput and performance improve
- Separate TID read operations are no longer required
- Feature remains enabled across reader sessions until disabled
