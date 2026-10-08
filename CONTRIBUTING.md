# Contributing to KR Cold War

Thank you for your interest in contributing to KR Cold War: The Long Armistice!

## Development Guidelines

### Code Style

- **Events**: Use namespaced IDs (e.g., `krcw_china.1`, `krcw_proxy.100`)
- **Focus trees**: Follow mutex layout patterns, avoid overly linear paths
- **Localization**: Keep text natural, avoid "AI-sounding" phrases
- **Balance**: Reference KR and TFR patterns for rewards and timing

### Common Pitfalls

1. **National Focus Scores**: Always include `ai_will_do` with proper scoring
2. **Character Promotion**: Use `promote_character` correctly with role assignments
3. **Equipment Transfers**: Validate `send_equipment` sender/receiver logic
4. **Duplicate IDs**: Check for ID conflicts across all namespaces

### Project Structure

```
kr_cold_war/
├── common/           # Game definitions
│   ├── decisions/    # Decision categories and actions
│   ├── ideas/        # National spirits and modifiers
│   ├── national_focus/ # Focus trees
│   └── ...
├── events/           # Event files
├── history/          # Starting conditions
├── interface/        # GUI definitions
├── localisation/     # Text and translations
└── gfx/             # Images and graphics
```

## Submitting Changes

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Make your changes following the style guidelines
4. Test in-game (load to at least 1951.1.1)
5. Commit with clear messages
6. Push and create a Pull Request

## Testing Checklist

- [ ] No errors in error.log
- [ ] Focus tree displays correctly
- [ ] Events fire as intended
- [ ] Localization keys all resolve
- [ ] AI behavior seems reasonable

## Questions?

Open an issue or reach out via Steam Workshop comments.
