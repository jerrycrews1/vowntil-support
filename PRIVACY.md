# Vowntil Privacy Policy

Effective date: July 14, 2026

Vowntil is a free Screen Time commitment app provided by Nerdquad. This policy explains how Vowntil handles information when you use the iOS app.

## Summary

Vowntil does not require an account and does not collect, sell, rent, track, or transmit your personal data to Nerdquad. The app has no advertising SDK, analytics SDK, or Nerdquad backend connection.

Vowntil uses Apple system frameworks to perform its core features. App selections, schedules, saved location automations, lock history, settings, and related operational records are stored locally on your device. Screen Time usage reports are prepared and displayed through Apple's privacy-preserving Device Activity report extension. Place searches are processed by Apple Maps.

## Information Vowntil Handles on Your Device

Vowntil may process the following information locally to provide features you request:

- Screen Time authorization status.
- Private tokens for apps, app categories, and websites selected through Apple's Family Activity picker.
- Named presets, app and website restriction modes, schedules, lock start and end times, and app settings.
- Saved location-automation names, place labels, coordinates, radii, enabled states, entry times, and active-region identifiers.
- Local lock History and enforcement events, including authorization changes, location entry or exit events, and whether a scheduled or manual lock completed or was interrupted.
- Screen Time usage information Apple makes available to the Device Activity report extension, such as usage duration, pickups, notifications, app categories, and websites.
- App version, iOS version, timestamps, session identifiers, and selection counts included in a diagnostics file only when you choose to export one.

Nerdquad does not receive this information from the app.

## Screen Time and Apple Services

Vowntil uses Apple's Family Controls, Managed Settings, Device Activity, and User Notifications frameworks. Apple controls Screen Time authorization, the private app and website picker, enforcement at the operating-system level, usage-report availability, and notification delivery.

Apple may process device and Screen Time information under Apple's own terms and privacy policy. Vowntil does not receive your Apple ID credentials or Screen Time passcode.

## Location and Apple Maps

Location access is optional and is used only when you create or enable a location automation. Vowntil asks for When In Use access first and then for Always access because iOS requires Always access to deliver region-boundary events while the app is not in use.

Vowntil stores saved place coordinates, radii, and current region-entry state in its local app-group container so the app and its extensions can apply your chosen preset. Vowntil does not continuously record a route or location history and does not send saved locations to Nerdquad.

When you search for a place, the search text and related request information are sent to Apple Maps by Apple's MapKit framework. Apple processes that information under its own terms and privacy policy. After you choose a result, Vowntil locally saves the selected place label and coordinates. You can delete a saved location automation in the app and can remove location access in iOS Settings.

## Local Notifications

If you grant notification permission, Vowntil schedules and delivers local notifications for lock-related events. Vowntil does not use a Nerdquad push-notification server and does not transmit notification content to Nerdquad.

## Diagnostics You Choose to Export

Vowntil can create a diagnostics file on your device when you explicitly request one. The file can contain app and iOS versions, authorization status, timestamps, session identifiers, selection counts, active-lock details, and recent local enforcement events. It does not include saved coordinates or Apple Maps search text.

Vowntil does not upload that file automatically. You decide whether, where, and with whom to share it through the iOS share sheet. Any third-party service you choose for sharing processes the file under its own privacy terms. Review the file and remove anything you do not want to share before sending it. Do not post diagnostics in a public GitHub issue.

## Data Collection, Tracking, and Advertising

Vowntil does not:

- Collect data from the app for Nerdquad.
- Track you across apps or websites.
- Use advertising identifiers.
- Display third-party advertising.
- Include third-party analytics or crash-reporting SDKs.
- Sell or share personal data for targeted advertising.

## Storage, Retention, and Deletion

Vowntil stores its operational data in the app's local iOS and shared app-group containers so the main app and its extensions can work together. Local History can be cleared using available in-app controls. Removing Vowntil normally removes its local app data from the device, subject to Apple's iOS and backup behavior.

Your device, Apple services, or device backups may retain information according to your Apple settings and Apple's policies. Nerdquad cannot access or delete data held only on your device or by Apple.

## Security

Vowntil relies on iOS sandboxing, app-group access controls, code signing, and Apple's Screen Time privacy protections. No method of storage is guaranteed to be completely secure, but the app minimizes risk by avoiding accounts, advertising, analytics, and transmission of your data to Nerdquad.

## Children

Vowntil does not knowingly collect personal data from anyone, including children. The app is a self-control tool and is not represented as parental monitoring or device-management software.

## Public Support Site

These support and privacy pages are hosted on GitHub. Visiting them is separate from using the Vowntil app, and GitHub may process web-access information under the [GitHub Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

## Changes to This Policy

This policy may be updated when Vowntil's features or data practices change. Material changes will be posted in this repository with a revised effective date. Vowntil's App Store privacy disclosures will be updated when required.

## Contact and Privacy Requests

For support or a privacy question, [open a GitHub issue](https://github.com/jerrycrews1/vowntil-support/issues/new/choose). Do not include private Screen Time selections, website activity, diagnostics files, or other sensitive information in a public issue.
