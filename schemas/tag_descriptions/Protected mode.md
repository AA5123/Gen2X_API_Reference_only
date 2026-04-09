**Protected Mode**

Impinj Protected mode is a security feature that makes an RFID tag invisible to all readers unless the reader first provides the correct 32-bit PIN/password. This prevents unauthorized access, reading, or cloning of the tag. You can use the following APIs to enable or disable protection, control tag visibility, and restrict tag responses to short-range only.

**Key Features:**
- **Tag Protection**: Lock individual tags with a 32-bit password making them RF silent and invisible
- **Tag Visibility**: Allow authorized readers to see protected tags by providing the correct password
- **Short-Range Mode**: Restrict protected tags to respond only at close proximity to the antenna
- **Password Authentication**: Secure tag access with 8-character hexadecimal passwords

**Related Commands:**
- `enable_tag_protection`: Lock a tag with a 32-bit access password
- `disable_tag_protection`: Remove protection and restore normal tag operation
- `enable_tag_visibility`: Authorize the reader to see protected tags
- `disable_tag_visibility`: Revoke reader authorization for protected tags
- `enable_short_range`: Protect a tag and restrict to short-range response only

**Use Cases:**
- **Retail Security**: Prevent tag cloning and unauthorized merchandise tracking
- **Warehouse Management**: Protect high-value asset tags from theft
- **Point-of-Sale**: Ensure only intended tags are read at checkout with short-range mode
- **Access Control**: Selectively grant reader access to specific protected tags

