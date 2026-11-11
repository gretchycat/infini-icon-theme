# Infini Icon Theme

Canonical SVG artwork and deterministic tools for the InfiniFolder default icon
theme. The Gradle viewer modules consume `default theme/` directly and package
it into the application at build time.

## Build the importable theme

```sh
python3 icon/scripts/build_icon_theme.py
```

This writes `exports/infinifolder-default.zip`. To prepare the bundled Android
assets and generated Kotlin sources, pass `--assets-dir` and `--kotlin-dir`;
the InfiniScribe and InfiniFolder viewer builds do this automatically.

To regenerate the artwork from the checked-in bases and reviewed inventory:

```sh
python3 icon/scripts/generate_icons.py
```

Python 3.9 or newer is required.
