# Quinnerary Privacy Policy

**Effective:** May 1, 2026
**Last updated:** May 1, 2026

Quinnerary is a personal travel itinerary app that turns confirmation
screenshots into a structured trip plan. We've designed it to keep your
data on your device by default. This page explains what happens with
your data.

## Summary

- Your trips, segments, flights, lodgings, and events live **locally
  on your device** in SwiftData. They are not uploaded to any server we
  control.
- When you use **Smart Scan**, the screenshot you select is sent to
  Anthropic's Claude API for parsing. The screenshot is processed by
  Anthropic and returned as structured fields. Quinnerary does not
  retain a copy on any server.
- When you use **Activity ideas** (free-time suggestions), the
  destination location, time window, and a brief description are sent
  to Anthropic to generate suggestions.
- We do **not** collect analytics, advertising identifiers, or
  telemetry. There are no third-party SDKs in the app beyond Apple's
  own frameworks.

## Information we access on your device

| Data | Why | Where it lives |
|---|---|---|
| Photos in the "Quinnerary" album | To detect new screenshots and extract their travel content | On your device, accessed only when the app is open |
| Your Anthropic API key | To call Claude on your behalf for Smart Scan and activity ideas | iOS Keychain on your device |
| Trip / segment / item data you save | To display your itinerary | On-device SwiftData store |
| Photos taken during your trip dates | To suggest a cover image for the trip | Read transiently; only the asset's identifier is saved, not a copy |

## Information sent to third parties

### Anthropic (Claude API)

When you trigger Smart Scan, the **selected screenshot image** is sent
to Anthropic's API for vision-based parsing. When you tap "Activity
ideas" on a free-time card, the **destination text and time window**
are sent. Anthropic's privacy practices govern that data once it
leaves your device:

- Anthropic privacy policy: https://www.anthropic.com/privacy
- Anthropic API data usage: https://www.anthropic.com/api

You provide your own Anthropic API key in Settings. The key is stored
in your device's iOS Keychain and is never sent anywhere except to
Anthropic in the standard `x-api-key` header.

### Apple

Apple Maps is used to render trip cover snapshots and the Visited tab
map. Apple's geocoding service is used to convert addresses to
coordinates. Apple's standard privacy practices apply.

## What we do not do

- We do **not** sell, rent, or share your data with anyone.
- We do **not** use any third-party analytics, advertising,
  attribution, or tracking SDKs.
- We do **not** create user accounts or operate a server backend.
- We do **not** read photos outside the dedicated "Quinnerary" album
  unless you explicitly pick one (e.g. "Set cover photo" in the trip
  menu).

## Your control

- **Delete a trip, segment, or item** at any time via the app's UI.
  This removes it from the on-device store immediately.
- **Revoke Photos access** in iOS Settings → Privacy → Photos →
  Quinnerary at any time. The app will gracefully degrade to manual
  entry only.
- **Remove your API key** in Quinnerary Settings → Anthropic API key
  → clear the field. Smart Scan and Activity ideas will stop calling
  Claude.
- **Uninstall the app** to remove all on-device data. Nothing remains
  on any server we operate, because there is no such server.

## Children's privacy

Quinnerary is not directed to children under 13 and does not knowingly
collect data from children.

## Changes

If we materially change how we handle data, we'll update this page
and bump its "Last updated" date.

## Contact

Questions, concerns, or data requests: **quinnmefford@gmail.com**
