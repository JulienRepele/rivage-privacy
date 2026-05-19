---
layout: default
title: Rivage — Privacy Policy
description: Privacy policy for the Rivage Android app.
---

# Privacy Policy

**Effective date:** 2026-05-19
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

---

## Quality monitoring (Firebase)

To detect crashes, monitor performance and understand which features are useful, Rivage uses **Firebase by Google** — specifically Firebase Crashlytics, Firebase Analytics and (optionally) Firebase Performance Monitoring.

What Firebase receives:

- **Crash reports** — stack traces, device model, OS version, app version, language, and the time of the crash. Necessary to fix the bug.
- **Anonymous usage events** — which screens you open, which buttons you tap, session duration. We use this in aggregate to decide which features to keep, improve or retire.
- **Coarse, IP-derived location** — Google may derive a country-level / region-level location from the IP address of the request. This is **not** the GPS location the app uses to compute tides; the GPS location is never forwarded to Firebase.
- **Pseudonymous identifier** (Firebase Installation ID, and possibly the Android Advertising ID) so events can be aggregated per device without identifying you personally.

What Firebase does **not** receive:

- Your stored favorites, recent searches, or any content you've entered into the app.
- The precise GPS coordinates used inside the app.
- Your email, name, or any other directly identifying information — Rivage does not collect those in the first place.

Firebase's processing is governed by Google's privacy policy: <https://policies.google.com/privacy>. You can reset or opt out of the Android Advertising ID at any time in your device settings (Settings → Privacy → Ads).

---

## Advertising

Rivage may display advertising in future releases to help fund development. If advertising is added, this policy will be updated to specify the advertising network used, what it collects, and how to opt out of personalised ads (typically by resetting the Android Advertising ID in your device settings).

---

## What Rivage does **not** do

- No account creation, no login, no email collection.
- No background data collection of your location. The app only fetches tides, weather and marine data in response to a foreground user action or a scheduled widget refresh.
- No data is sold or rented to data brokers.
- No precise GPS location is sent to anyone other than the third-party APIs above, and only in the moment you request a forecast for that point.

---

## Children

Rivage does not knowingly collect any personal information from children under 13. The app is rated for general audiences and does not require an account.

---

## Changes to this policy

If the data-handling practices change in a future version of the app, this page will be updated and the **Effective date** at the top will be revised. Material changes will also be mentioned in the app's release notes on Google Play.

---

<sub>This document is hosted as a static page on GitHub Pages and is also accessible directly inside the app's settings screen.</sub>
