# Flutter Analyze `pre-commit`

[`pre-commit`](https://pre-commit.com) hook for running Flutter anlyzer

Add the following in your `.pre-commit-config.yaml`:
```yaml
  - repo: https://github.com/mcsken/flutter-analyze-pre-commit
    rev: v0.1
    hooks:
      - id: dart-format
        args: [--line-length=120] # Extends the dart code length to 120 from the default of 80.
      - id: flutter-analyze
        args: [your_app/lib/*]

```

## Acknowledgements

[Charles Crete](https://github.com/Cretezy/) for creating `flutter-format-pre-commit`
