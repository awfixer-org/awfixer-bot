# NOTICE: Project Architecture and Integration Goals

## Purpose
This notice outlines the strategic direction for integrating `discord.py` and `disgord` into the broader awfixer-bot project.

## Current State
- `discord.py/`: Python Discord library fork
- `disgord/`: Go Discord library implementation
- Both are being developed as part of a unified bot ecosystem

## Integration Goals
1. **Gradual Integration**: Slowly integrate both libraries into the main bot project
2. **API Architecture**: Write core API functionality in Go using `disgord`
3. **Bot Logic**: Implement main bot functionality in Python using `discord.py`
4. **Custom Implementation**: Move away from third-party libraries toward custom implementations
5. **Discord API Compatibility**: Ensure rapid adoption of new Discord API features

## Technical Strategy
- Go API layer for performance and low-level Discord API interaction
- Python layer for bot logic, commands, and user-facing features
- Custom implementations to control feature rollout and Discord API compatibility
- Focus on maintaining cutting-edge Discord API feature support

## Developer Guidelines
- When working with `discord.py` or `disgord`, consider integration impact
- Prioritize custom implementations over library dependencies
- Ensure compatibility between Go API layer and Python bot layer
- Document integration points and data flow between components

## Future Vision
Create a unified bot system with:
- Go-based high-performance API layer
- Python-based flexible bot logic
- Custom Discord API implementations
- Rapid feature deployment capability

---
*This notice should be referenced when making architectural decisions or when working on integration between components.*