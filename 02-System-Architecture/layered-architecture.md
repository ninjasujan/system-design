#### Layered Architecture

**Layers**

1. UI Interface
2. Authorization layer
3. Business Logic
4. OS and DB Layer

- Lower layers never call upper layers.
- Request cycle always starts from the upper layer.
- Easy to add security features at different layer levels.
- Easy to build on top of layers due to clear separation and no coupling.
- Performance issues may arise due to several layers.
