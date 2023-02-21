# Flutter Format `pre-commit`

[`pre-commit`](https://pre-commit.com) hook for formatting Flutter files.

Add the following in your `.pre-commit-config.yaml`:
```yaml
- repo: https://github.com/guy-av/flutter-format-pre-commit
  rev: "master"
  hooks:
    - id: flutter-format
```

You can also only include/exclude some files (defaults to only `.dart`, is a pattern):

```yaml
- repo: https://github.com/guy-av/flutter-format-pre-commit
  rev: "master"
  hooks:
    - id: flutter-format
      files: lib/* # Only format source files
      exclude: lib/src/avatar.dart # Exclude the avatar widget
```

## Dart

Also see [Dart Format `pre-commit`](https://github.com/Cretezy/dart-format-pre-commit) for formatting only Dart code.
