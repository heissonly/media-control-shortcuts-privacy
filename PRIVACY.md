# Privacy Policy for Media Control Shortcuts

Effective date: August 16, 2026
Extension display version: 1.3

Media Control Shortcuts controls audio and video playback in Chrome. Its single purpose is to let the user operate media through browser-wide shortcuts and pointer-based volume control.

## Data handled by the extension

To provide that user-facing function, the extension processes the following information locally in the browser:

- The URLs and audible/active state of open tabs, only to identify the requested media tab and honor the user's excluded-sites list.
- Media-element state such as playing, paused, volume, mute state, current time, duration, and playback rate, only to execute and verify a media command.
- User shortcut and wheel interactions, only when they invoke an extension feature.
- User preferences stored by the extension: excluded hostnames, recent media tab/frame identifiers and activity timestamps used for resume routing, and the last extension-selected Facebook Reels volume/mute preference.

The extension does not read page text, form entries, passwords, authentication cookies, private messages, payment information, or the audio/video stream itself.

## Local processing and storage

All processing occurs on the user's device. Preferences and recent routing state are stored with `chrome.storage.local`. Media state and tab URLs used for routing are evaluated locally and are not sent to the developer or any third party.

The user can remove locally stored extension data by removing the extension or clearing its extension storage. Individual excluded hostnames can be removed from the extension popup.

## Data collection, transmission, and sharing

Media Control Shortcuts:

- does not transmit user data to external servers;
- does not use analytics, telemetry, advertising, tracking pixels, or crash-reporting services;
- does not sell, rent, share, or disclose user data to third parties;
- does not use user data for advertising, creditworthiness, or any purpose unrelated to media control;
- does not allow the developer or other humans to read the user's browsing or media data;
- does not execute remotely hosted code.

## Chrome Web Store Limited Use disclosure

The use of information received from Chrome APIs adheres to the Chrome Web Store User Data Policy, including the Limited Use requirements. Information is used only to provide or improve the extension's single, user-facing media-control purpose.

## Permissions

- **tabs:** identifies audible, active, or recently used media tabs; reads the current tab URL only for routing and excluded-site checks; sends commands to the selected tab.
- **commands:** receives the keyboard shortcuts configured by the user in Chrome.
- **storage:** keeps excluded sites, recent media-routing state, and the Facebook Reels volume preference locally.
- **webNavigation:** enumerates frames so a command reaches the exact frame containing the media instead of every frame in a tab.
- **Website access:** detects and controls HTML audio/video players on pages where the user invokes the extension. Broad website access is required because media may appear on any website or embedded frame.

## Changes to this policy

This policy will be updated when the extension's data practices change. Material changes will be disclosed in the Chrome Web Store listing and in an updated policy before the new practices take effect.

## Contact and support

Questions, privacy requests, and support reports can be submitted at:

https://github.com/heissonly/media-control-shortcuts-privacy/issues
