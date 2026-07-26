# iPhone Health Sleep Shortcuts

An iPhone-only sleep-logging workflow that records manually confirmed
sleep sessions in Apple Health using Apple Shortcuts.

No Apple Watch, paid subscription, external server, or third-party
sleep-tracking service is required.

![Project icons](assets/icons/start-sleep.PNG)

## What It Does

The project contains two coordinated shortcuts:

### Sleep — Start

- Records the beginning of a sleep session
- Creates or updates a temporary timestamp marker
- Activates Sleep Focus
- Displays a confirmation notification

### Sleep — Finish

- Retrieves the sleep-start timestamp
- Records the current wake time
- Asks for estimated sleep latency
- Logs an `In Bed` interval into Apple Health
- Logs an `Asleep` interval into Apple Health
- Turns Sleep Focus off

## Requirements

- An iPhone with the Shortcuts app
- Apple Health
- iCloud Drive
- Sleep Focus configured
- Permission for Shortcuts to write Sleep data

## Installation

See [Installation Guide](docs/installation.md).

## Daily Usage

### At night

Run:

`Sleep — Start`

when you are actually ready to sleep.

### In the morning

Run:

`Sleep — Finish`

when you are actually getting up.

Enter an estimate of how many minutes it took you to fall asleep.

## Screenshots

### Shortcut controls

![Control Center](assets/screenshots/home-screen.HEIC)

### Apple Health result

![Apple Health result](assets/screenshots/sleep_apple-health-2.HEIC)

## Privacy

- No sleep data is sent to an external server.
- No advertising or analytics service is used.
- Permanent sleep records are stored in Apple Health.
- The temporary marker file is stored in the user's iCloud Drive.
- Each user controls the Health permissions granted to Shortcuts.

See [Privacy Information](docs/privacy.md).

## Important Limitations

This project does not:

- Automatically detect when you fall asleep
- Measure REM, Core, or Deep sleep
- Detect unreported nighttime awakenings
- Replace an Apple Watch or medical sleep study
- Provide medical advice or diagnosis

Sleep latency is manually estimated by the user.

## Project Files

```text
shortcuts/
├── Sleep-Start.shortcut
└── Sleep-Finish.shortcut
```

## Troubleshooting

See [Troubleshooting Guide](docs/troubleshooting.md).

## Version

Current stable release: `v1.0.0`

See [CHANGELOG.md](CHANGELOG.md).

## License

This project is released under the MIT License.

## Maintainer

Created and maintained by @ClapItsMe.
