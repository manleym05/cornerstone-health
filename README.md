# Cornerstone Health

A personal health dashboard. Connect your Öura ring, and Cornerstone Health shows you your
daily readiness and sleep trends in one place.

**Status: development.** This is a personal project, currently used by its author only. It is
not open for signups.

## What it does

Once you connect your Öura account, Cornerstone Health checks in once a day and records a
short summary of that day:

- Readiness score
- Sleep score
- HRV balance
- Resting heart rate

That's it. It reads those daily summaries and nothing else.

## What it doesn't do

- It doesn't sell, share, or transmit your data to any third party.
- It doesn't run ads, analytics, or tracking.
- It doesn't write anything back to your Öura account — access is read-only.
- It doesn't read your workouts, tags, SpO2, stress, heart-health, or ring-configuration data.
  Those permissions are deliberately not requested.

## How your Öura account is connected

Connecting uses Öura's standard OAuth flow. You authenticate with Öura directly — Cornerstone
Health never sees your Öura password. Öura returns a token that is encrypted and stored on the
server side only; it is never sent to your browser or stored on your device.

You can disconnect at any time from your
[Öura account's connected applications](https://cloud.ouraring.com/), which immediately revokes
access.

## Documents

- [Privacy Policy](PRIVACY.md)
- [Terms of Service](TERMS.md)

## Contact

manleym05@gmail.com
