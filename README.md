# FocusTomato

[简体中文](README_zh.md) | English

FocusTomato is a native macOS website and app blocker for focused work. Start a focus session, schedule recurring protected time, and keep distracting websites and apps out of the way.

![FocusTomato Blue theme interface](https://alexab612.github.io/FocusTomatoDoc/img/screenshot.png)

- [Website](https://alexab612.github.io/FocusTomatoDoc/)
- [Download v1.0.3](https://github.com/alexab612/FocusTomato/releases/tag/v1.0.3)
- [Privacy Policy](https://alexab612.github.io/FocusTomatoDoc/privacy/)
- [Terms of Use](https://alexab612.github.io/FocusTomatoDoc/terms/)
- [Feedback and Support](https://github.com/alexab612/FocusTomato/issues)

### Download

Current stable version: **v1.0.3**

- [Download FocusTomato-1.0.3.dmg](https://github.com/alexab612/FocusTomato/releases/download/v1.0.3/FocusTomato-1.0.3.dmg)
- [View the v1.0.3 release notes](https://github.com/alexab612/FocusTomato/releases/tag/v1.0.3)
- [View all releases](https://github.com/alexab612/FocusTomato/releases)

### Installing on macOS

1. Download and open the DMG, then drag `FocusTomato` into the `Applications` folder.
2. This build is not currently signed with Developer ID or notarized by Apple. On first launch, macOS may block it because the developer cannot be verified.
3. If it is blocked, open `System Settings -> Privacy & Security -> Security`, locate the message about FocusTomato, and click **Open Anyway**.
4. Confirm **Open** in the macOS dialog. The app can then be launched normally.

Website blocking requires macOS Automation permission. The first time FocusTomato needs to block sites in a browser, allow it to control that browser when prompted. You can review this permission under `System Settings -> Privacy & Security -> Automation`.

### Features

- Website and app rules: Each preset supports a separate blocklist or allowlist for websites and apps.
- Per-item control: Disable an existing list item with its checkbox without deleting it.
- Focus and breaks: Run timed focus sessions with pause, resume, and post-session break flow.
- Recurring schedules: Activate preset rules automatically by weekday and time period.
- Statistics: Review focused time, session counts, and most-blocked websites or apps.
- Menu bar controls: Check status and control the current session from the menu bar.
- Update checking: Manually check GitHub Releases for newer app versions.
- Appearance: Choose System, Light, Dark, or the colorful `Blue` theme.

### Supported Browsers

Website blocking currently supports `Safari`, `Google Chrome`, `Microsoft Edge`, `Brave`, `Opera`, and `Arc`. App blocking applies to the macOS apps added to your presets.

### Privacy

The current version of FocusTomato is local-first. Settings, presets, focus-session history, and statistics are stored on your Mac. The app does not include accounts, remote analytics, or advertising trackers. Cloud sync is not available in the MVP version.

[Read the full Privacy Policy](https://alexab612.github.io/FocusTomatoDoc/privacy/)

### Terms

FocusTomato uses Apple's Standard End User License Agreement as its baseline license, with concise supplemental app-specific terms.

[Read the full Terms of Use](https://alexab612.github.io/FocusTomatoDoc/terms/)

### Feedback and Support

For bug reports and feature requests, please use [GitHub Issues](https://github.com/alexab612/FocusTomato/issues).

### Local Development

Build the macOS app:

```bash
xcodebuild -project FocusTomato.xcodeproj -scheme FocusTomato -configuration Debug -destination 'platform=macOS' build
```

Build the documentation site:

```bash
cd FocusTomatoDoc
npm install
npm run build
```
