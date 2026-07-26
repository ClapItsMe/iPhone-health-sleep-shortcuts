
# Troubleshooting

## Marker File Not Found

Confirm that both shortcuts use:

SleepTracker/sleep-start.txt

## Health Entry Does Not Appear

Verify that Shortcuts has permission to write Sleep data in Apple Health.

## Start Time Is Incorrect

Do not manually edit or reopen the marker file during the sleep session.

Do not run `Sleep — Start` twice during the same night.

## Invalid Sleep Interval

During a short test, enter `0` minutes for sleep latency.

The estimated latency cannot be longer than the entire test session.

## Sleep Focus Does Not Change

Verify the `Set Focus` actions:

- Start Shortcut: Turn Sleep Focus on
- Finish Shortcut: Turn Sleep Focus off
