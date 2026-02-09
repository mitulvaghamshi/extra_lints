# extra_lints

This package offers additional linter rules for Dart and Flutter projects.

## Usage

To incorporate this package into your project, add the following to your [pubspec.yaml](example/pubspec.yaml).

```yaml
dev_dependencies:
  extra_lints:
      git:
        url: https://github.com/mitulvaghamshi/extra_lints.git
```

Next, add the following to your [analysis_options.yaml](example/analysis_options.yaml):

For Flutter projects:

```yaml
include: package:extra_lints/flutter.yaml
```

For Dart projects:

```yaml
include: package:extra_lints/dart.yaml
```

## Notes:

- By using the `extra_lints` package, you can remove the `lints` and/or `flutter_lints` packages from your `pubspec.yaml` as this package automatically incorporates rules from `package:flutter_lints/flutter.yaml` when `package:extra_lints/flutter.yaml` is included and `package:lints/recommended.yaml` rules when `package:extra_lints/dart.yaml` is included in your `analysis_options.yaml` file.
- If you prefer to retain the `lints` and/or `flutter_lints` packages, you can simply include `package:extra_lints/extra.yaml` in addition to `package:lints/recommended.yaml` and/or `package:flutter_lints/flutter.yaml` in your `analysis_options.yaml` file.

## Lint Set Contents

Refer to [extra.yaml](lib/extra.yaml) for a comprehensive list of rules that constitute the extra rule set.
