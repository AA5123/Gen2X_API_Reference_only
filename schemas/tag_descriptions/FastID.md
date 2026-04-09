**FastID**

Use FastID to receive both the EPC (Electronic Product Code) and TID (Tag Identifier) in a single inventory response. This eliminates the need for a separate TID read operation and significantly improves inventory throughput and efficiency.

**Key Features:**
- **Dual Data Retrieval**: Capture both EPC and TID in a single RF exchange
- **Enhanced Throughput**: Reduce inventory time by eliminating redundant reads
- **Improved Efficiency**: Decrease RF transmissions and overall reader load
- **Simplified Protocol**: Single command retrieves all essential tag identifiers

**Related Commands:**
- `enable_fastid`: Enable FastID feature for dual EPC/TID responses
- `disable_fastid`: Return to standard EPC-only inventory responses

**Performance Benefits:**
- Reduces inventory round time by up to 50% when TID data is needed
- Decreases RF overhead and power consumption
- Improves tag read rates in dense environments
- Simplifies data processing by combining two data fields

**Use Cases:**
- **Item Authentication**: Verify both EPC and TID for product authentication
- **Inventory Audit**: Complete tag identification in single scan
- **High-Speed Processing**: Maximize throughput in fast-moving applications
- **Data Collection**: Gather comprehensive tag metadata efficiently
