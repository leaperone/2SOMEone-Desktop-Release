# 2SOMEone Desktop Release

This repository handles automated builds and releases for [2SOMEone Desktop](https://github.com/leaperone/2SOMEone-Desktop).

## Download

Download the latest release from the [Releases](https://github.com/leaperone/2SOMEone-Desktop-Release/releases) page.

| Platform | Download |
|----------|----------|
| macOS (Apple Silicon) | `.dmg` |
| macOS (Intel) | `.dmg` |
| Windows | `.exe` |
| Linux | `.AppImage` / `.deb` |

## Auto Update

The app supports auto-update. Updates are served from:
- https://static.2some.ren/release/2someone-desktop/

## Manual Build Trigger

1. Go to [Actions](https://github.com/leaperone/2SOMEone-Desktop-Release/actions)
2. Select "Build and Release" workflow
3. Click "Run workflow"
4. Enter the version tag (e.g., `1.0.0-build.1`)
5. Select platforms to build
6. Click "Run workflow"

## Build Matrix

| Platform | Runner | Build Output |
|----------|--------|--------------|
| macOS | `macos-latest` | `.dmg`, `.zip` |
| Windows | `windows-latest` | `.exe` |
| Linux | `ubuntu-latest` | `.AppImage`, `.deb` |

## Secrets Required

The following secrets must be configured in this repository:

| Secret | Description |
|--------|-------------|
| `BITIFUL_ACCESS_KEY_ID` | S3 Access Key |
| `BITIFUL_SECRET_ACCESS_KEY` | S3 Secret Key |

## License

See the main repository for license information.
