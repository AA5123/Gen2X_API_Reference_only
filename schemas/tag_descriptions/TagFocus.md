**TagFocus**

Use TagFocus to improve read rates in dense tag environments. After a tag is inventoried, it stays silent in subsequent rounds so the reader can focus on new or unread tags. TagFocus targets tags in session S1.

**Key Features:**
- **Smart Tag Filtering**: Already-inventoried tags automatically suppress responses
- **Focused RF Energy**: Reader concentrates on discovering new tags
- **Improved Throughput**: Eliminate duplicate reads and wasted RF cycles
- **Session Management**: Applies to Session S1; resets on new session
- **Adaptive Inventory**: Automatic handling without tag-specific configuration

**Related Commands:**
- `enable_tagfocus`: Activate TagFocus to suppress previously read tags
- `disable_tagfocus`: Return to standard inventory mode with all tags responding

**Performance Improvements:**
- Increases read rate by 30-50% in high-density tag environments
- Reduces inventory time for discovering new tags
- Optimizes RF energy utilization
- Minimizes duplicate read overhead

**Session Behavior:**
- Active within Session S1 inventory operations
- Resets when reader stops and restarts
- Accumulates read tags throughout session
- Compatible with other Gen2X features

**Use Cases:**
- **Large-Scale Inventory**: Speed up discovery of new tags in crowded spaces
- **Asset Tracking**: Focus detection on new asset arrivals
- **Warehouse Operations**: Improve throughput in aisles with many tags
- **Distribution Centers**: Accelerate receiving and shipping operations
