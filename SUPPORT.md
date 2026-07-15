# Vowntil Support

Vowntil is a free commitment tool that uses Apple's Screen Time frameworks to restrict apps, categories, and websites during a Hard Lock or an automation you create.

## Get Help

For a bug, unexpected behavior, or feature request, [open a support issue](https://github.com/jerrycrews1/vowntil-support/issues/new/choose).

Before posting, please:

- Check that your device is running a supported version of iOS.
- Include your Vowntil version, iOS version, device model, and clear steps to reproduce the problem.
- Remove names, contact information, app selections, website details, and any other personal information from screenshots or text.
- Do not post a diagnostics file publicly. Diagnostics can contain session identifiers, timestamps, device and app versions, selection counts, and recent local enforcement events.

## Common Questions

### Why does Vowntil need Screen Time access?

Vowntil uses Apple's Family Controls, Managed Settings, and Device Activity frameworks to let you privately choose apps and websites, enforce a lock, run schedules, and display usage reports. Vowntil cannot perform those functions without Screen Time authorization.

### Why does the app picker look different from a normal app list?

Apple owns the Family Activity picker. Apps and websites are represented to Vowntil with private tokens, so Vowntil does not receive a conventional list of every installed app or the identity of selections outside Apple's approved interfaces.

### Can apps and websites use different restriction modes?

- **Block Selected** shields only the apps, categories, or websites you choose.
- **Allow Only Selected** shields everything covered by Screen Time except the apps or websites you choose to keep available.
- **Same as Apps** makes the website mode follow the app mode.

For example, you can allow only selected apps while blocking only selected websites, or block selected apps while allowing only a small set of websites. Review both summary rows carefully before starting a Hard Lock.

### Can Vowntil end a Hard Lock early?

Vowntil does not provide an in-app pause, password reset, recovery code, Face ID override, or support unlock. A Hard Lock ends at its scheduled time.

Vowntil is not device-management software. The device owner can still remove Vowntil's Screen Time authorization in iOS Settings or erase the device. Removing authorization causes iOS to stop Vowntil's restrictions. When Vowntil detects this during a lock, it records the interruption in local History and can send a local notification if notifications are enabled.

### How do location automations work?

A location automation applies one of your presets when iOS reports that the device entered a saved circular region. It stops after iOS reports that the device exited. Vowntil stores the saved coordinates, radius, and entry state locally; it does not send them to Nerdquad.

Location automations require **Always** location access so iOS can deliver region events when Vowntil is not on screen. Vowntil monitors at most 20 enabled locations, which is the iOS limit. A manual Hard Lock takes priority over every automation. If regions overlap, the most recently entered enabled location takes priority over a time schedule.

### Why did a scheduled or location lock not start?

Confirm that:

- Screen Time authorization is active.
- The automation is enabled and has a preset assigned.
- The preset contains the intended app, category, or website selection.
- For a time schedule, the days and times are correct, including overnight schedules.
- For a location automation, Location Services and Always access are active and the radius covers the intended boundary.
- The device date, time, and time zone are correct.

Open Vowntil after changing authorization or major device settings so it can refresh its local state.

Apple's region monitoring is best effort. Boundary events can be delayed by device conditions, location accuracy, network availability, travel speed, restarts, or iOS behavior. Force-quitting Vowntil can also prevent iOS from relaunching it for a region event until the app is opened again. Location automations are a convenience for self-control, not a safety or security boundary.

### Why is the Usage tab empty or delayed?

Usage reports come from Apple's Device Activity system. Make sure Screen Time access remains active, select the intended date range and device scope, and allow time for iOS to process recent activity. Vowntil cannot invent or independently reconstruct usage that Apple has not made available to its report extension.

### How do I reset local data?

Use Vowntil's in-app controls to clear History where available. Removing Vowntil also removes its active app installation and normally removes its local container data, subject to Apple's device and backup behavior. Reinstalling does not restore an active lock that was removed with the app.

## Safety and Limitations

Vowntil is designed for self-control, not parental control, employee monitoring, emergency access control, location tracking, or permanent device management. Do not block apps or websites you may need for health, safety, travel, authentication, work, school, or emergencies.

## Privacy

Vowntil does not require an account, include ads or analytics SDKs, or send app data to a Nerdquad backend. See the full [Vowntil Privacy Policy](PRIVACY.md).

Last updated: July 14, 2026
