## disable_tagfocus

**Description:**
Disables the TagFocus feature, returning tags to normal operational mode where all tags respond to every inventory round regardless of prior reads.

**Usage:**
Send this command to deactivate TagFocus on the reader. Once disabled, all tags will respond to every inventory round, even if they were previously read in the current session. This is useful when you need to track tag movement, verify tag presence continuously, or when inventory redundancy is more important than throughput optimization.

**Parameters:**
- `enabled` (boolean): Set to `false` to disable TagFocus feature

**Behavior:**
- All tags respond to every inventory round
- Previously read tags return to normal response mode
- Duplicate reads reappear in inventory results
- No tag-level state management for reads
- Reader processes all responding tags equally
