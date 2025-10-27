---
layout: page
title: Norigoro Privacy Policy
description: Privacy Policy for Norigoro Bus Timer app
lang: en
---

Last Updated: October 28, 2025

This Privacy Policy (the "Policy") defines how Norigoro Bus Timer (the "App") handles user information.

Please read this Policy before using the App.

Language: [日本語](/apps/norigoro/privacy/) | English

Note: In case of discrepancies between the Japanese and English versions, the Japanese version shall prevail.

## 1. Information We Collect

The App collects the following information to provide bus arrival time display services.

### Location Information
- **Purpose**: To automatically detect nearest bus stops
- **Collection Method**: iOS Core Location API
- **Storage**: Device only (cached for 10 minutes)
- **External Transmission**: None (location data is never sent externally)

### Device-Related Information
- Language settings (obtained from system settings)
- System time (for arrival time calculations)

The App does **NOT** collect:
- Personally identifiable information
- Contacts, photos, camera, microphone
- Advertising IDs, tracking IDs
- Movement history, behavioral data

## 2. Collection Methods

- Through iOS Core Location API when user grants location permission
- Information from device system functions (time, language)

## 3. Purpose of Use

Collected information is used solely for the following purposes:

- Searching for and displaying nearest bus stops
- Calculating and displaying bus arrival times

## 4. Data Storage and Sharing

### Data Stored on Device

All data is stored only on the device and is never sent to external servers.

- **Location Cache**: Last obtained latitude/longitude (stored for 10 minutes only)
- **GTFS Data**: Bus routes, stops, and timetable data (obtained from Open Data Center for Public Transportation)
- **User Settings**: Display radius, time range, reference mode settings, last update time
- **Language Settings**: App display language (obtained from system settings)

### External Transmission

The App accesses the following API to obtain bus timetable data and real-time operation information.

#### Open Data Center for Public Transportation (ODPT) API
- **Information Sent**: None (location information is not sent)
- **Information Obtained**:
  - GTFS data (bus routes, stops, timetables)
  - GTFS-Realtime data (real-time delay information)
- **Data Source**: Open data from Kawasaki Tsurumi Rinko Bus Co., Ltd.
- **License**: Public Transportation Open Data Basic Terms of Use
- **Data Information**: https://developer.odpt.org/

The process of searching for nearest bus stops from location information is completed entirely on the device. Location information is never sent to servers.

### Third-Party Disclosure

We do not provide personal information to third parties except in the following cases:

- When required by law
- When necessary to protect life, body, or property and obtaining consent is difficult

The App does not use any third-party SDKs for advertising, tracking, or analytics.

## 5. Data Deletion

All data stored on the device will be deleted when you uninstall the App.

Methods to delete data from within the App:
- **Location Cache**: Automatically deleted after 10 minutes, or switch to reference mode
- **GTFS Data**: Uninstall the app
- **User Settings**: Uninstall the app

## 6. About Location Usage

### Purpose of Use
Location information is used only to automatically detect nearest bus stops.

### Collection Timing
- When app launches (if location permission granted)
- When screen is pulled down to refresh
- When returning from reference mode to normal mode

### Storage Period
Last obtained location information is cached for 10 minutes only. It is deleted after 10 minutes or when switching to reference mode.

### How to Stop Usage
1. Open iOS "Settings" app
2. Select "Privacy & Security" → "Location Services"
3. Select "Norigoro"
4. Select "Never"

Even if you stop location usage, you can check timetables at major stations using reference mode.

## 7. Security

The App implements the following measures to protect user information:

- Location information processed only on device, not sent externally
- Encrypted HTTPS communication
- Requests only minimum necessary permissions (location only)

## 8. Changes to Privacy Policy

This Policy may be changed without notice in response to legal changes or app feature additions. Important changes will be announced within the app.

The latest Privacy Policy is always available at:
https://ikeisuke.github.io/apps/norigoro/privacy/en/

## 9. Contact

For questions, comments, or requests regarding this Policy:

- Norigoro Contact: https://forms.gle/YSNCV67dmDPyedA3A

## 10. Disclosures

### Developer
Individual Developer: Keisuke Isono

### App Name
Norigoro Bus Timer

### Location
Japan

### Non-Affiliation Statement
This App is not affiliated with Kawasaki Tsurumi Rinko Bus Co., Ltd., the Open Data Center for Public Transportation, or any related public transportation operators. This is not an official app.

### Data Source
This App uses open data from Kawasaki Tsurumi Rinko Bus Co., Ltd. (provided by the Open Data Center for Public Transportation).

### Disclaimer
Timetable data and real-time information displayed in this App do not guarantee the accuracy or completeness of the data source. Please check bus stop timetables and official information for actual bus operations.

The developer assumes no responsibility for any damages arising from the use of this App.

---

This Privacy Policy is effective as of October 28, 2025.
