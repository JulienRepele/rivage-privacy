---
layout: default
title: Rivage — Privacy Policy
description: Privacy policy for the Rivage Android app.
---

# Privacy Policy

**Effective date:** 2026-05-18
**App:** Rivage (Android)
**Publisher:** Julien Repele

This page describes how the Rivage Android application handles your data. Rivage operates without any backend server owned by the publisher; the app talks directly to a small number of public weather and mapping APIs to render tide, wind and weather information.

---

## Data collected

### Location

Rivage uses your device's coarse or fine location **only when you explicitly enable it** through the Android permission prompt. Location is used for two purposes:

1. **"Current location" tile** on the home screen and the "Current location" button on the search screen — so the app can show tides, weather and nearby coastal cities for where you are.
2. **Nearby coastal cities search** — to populate the list of large cities and ports close to you.

Location coordinates are processed **entirely on your device**. They are passed to the third-party APIs listed below only as the latitude/longitude arguments needed to answer a specific query (e.g. "give me the tide forecast at 48.39, -4.49"). They are **never sent to a server owned or operated by Rivage's publisher** — there are no such servers.

You can revoke the location permission at any time in your device settings. Without it, the app still works for cities you search or favorite manually.

### Favorites, search history, settings

Favorites you add, recent searches, and your appearance / units preferences are stored **locally only**, in the app's private storage on your device. They are never transmitted anywhere. Uninstalling the app removes them.

---

## Third-party services

To compute tides, weather and search results, Rivage sends HTTPS requests to the following public APIs. Each request contains only the coordinates or query text needed to answer it, plus a generic `User-Agent` header identifying the app version.

| Service | Used for | Provider |
| --- | --- | --- |
| **Open-Meteo** ([open-meteo.com](https://open-meteo.com)) | Weather, marine (waves/swell) and tide forecasts | Open-Meteo non-commercial API |
| **Overpass API** ([overpass-api.de](https://overpass-api.de)) | Nearby coastal cities and ports | OpenStreetMap community |
| **Nominatim** ([nominatim.openstreetmap.org](https://nominatim.openstreetmap.org)) | City search by name (geocoding) | OpenStreetMap Foundation |

These providers receive the data necessary to answer your request (coordinates, search text). Their own privacy practices are governed by their respective policies:

- Open-Meteo: <https://open-meteo.com/en/terms>
- Nominatim / OpenStreetMap: <https://wiki.osmfoundation.org/wiki/Privacy_Policy>
- Overpass API: <https://wiki.openstreetmap.org/wiki/Overpass_API>

Rivage does not embed any analytics SDK, crash-reporting SDK, advertising SDK, or any other third-party library that performs background telemetry.

---

## What Rivage does **not** do

- No advertising tracking, no ad networks, no ad SDKs.
- No analytics SDK (no Firebase Analytics, no Crashlytics, no comparable tool).
- No persistent advertising identifier (Android Advertising ID) is read or transmitted.
- No account creation, no login, no email collection.
- No background data collection. The app only contacts external services in response to a foreground user action or a scheduled widget refresh.
- No data is sold, rented, or shared with third parties for marketing purposes.

---

## Children

Rivage does not knowingly collect any personal information from children under 13. The app is rated for general audiences and does not require an account.

---

## Changes to this policy

If the data-handling practices change in a future version of the app, this page will be updated and the **Effective date** at the top will be revised. Material changes will also be mentioned in the app's release notes on Google Play.

---

<sub>This document is hosted as a static page on GitHub Pages and is also accessible directly inside the app's settings screen.</sub>
