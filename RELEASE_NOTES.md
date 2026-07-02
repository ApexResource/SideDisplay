# Release Notes

## v1.10.0 (2026-07-03)

### New Features
- Redesign Connection mode: choose "Same network" or a single "Hotspot" with a "Share my internet" / "Screen only" option
- Screen-only hotspot (loopback) now works with Tesla — use it as a second display with no internet or tethering required
- Make the loopback adapter a one-time install that persists across sessions and reboots (no admin prompt every session); add a Remove action in Connection mode that also clears it from the System Settings Internet Sharing list
- Show live connection prerequisites (internet source, Wi-Fi, Internet Sharing) and verify Internet Sharing shares from the mode's expected source before enabling Start
- Rebuild the Getting Started guide around the new connection modes (Tesla flows start by resetting the car's Wi-Fi)

### Improvements
- Various DNS and hotspot stability fixes

## v1.9.1 (2026-04-21)

### Bug Fixes
- **Internet Sharing Compatibility** — Fixed NAT issue that caused "internet unreachable" errors on Tesla and other connected devices.

## v1.9.0 (2026-03-29)

### New Features
- **Per-Display Settings** — Each display now has independent configuration for resolution mode, scale, and auto-fullscreen. Manage displays via compact card UI with popover editor.
- **Display Selection Flow** — New display selection screen lets you choose which display to view after connecting. PIN verification now happens before display selection for added security.
- **Connection Status Redesign** — New clear status flow: Idle → Starting → Ready → Connected. Connected state shows active client count out of total displays.
- **Improved Scaling** — New scale options (1x / 1.25x / 1.5x / 1.75x) with browser-side GPU scaling for sharper output at higher scales.
- **File-Based Diagnostic Logging** — New diagnostic logging system captures app settings, network interfaces, bridge, DHCP, firewall rules, virtual displays, and DNS status on start.

### Improvements
- **Single Admin Prompt** — Bridge and DNS setup now combined into one password prompt instead of two.
- **Better Error Messages** — User-friendly errors for port conflicts and invalid license keys.
- **PIN Verification UX** — Red border with shake animation on incorrect PIN entry.

### Bug Fixes
- **WebRTC Stability** — Fixed scroll causing WebRTC disconnect due to sendBeacon flooding. Handle 'disconnected' state to prevent infinite reconnect loop.
- **Client Count** — Fixed connected client count not updating on browser or WebRTC disconnect.

## v1.8.1 (2026-03-17)

### Improvements
- **Enhanced Diagnostic Report** — Now includes app version, macOS version, and server status for more accurate troubleshooting.

## v1.8.0 (2026-03-17)

### New Features
- **Faster Connection** — Extended monitor connections are now significantly faster and more reliable.
- **Diagnostic Report** — Submit diagnostic reports directly from the app with optional email for follow-up support.

## v1.7.0 (2026-03-08)

### New Features
- **Always-on Domain Access** — The `go.ss` shortcut domain is now always active. No need to toggle it on manually.
- **Internet Access Control** — Control whether connected devices can access the internet through your hotspot. Disabled by default to save hotspot data.

## v1.5.1 (2026-02-26)

### New Features
- **Multi-Display Support** — Extend up to 3 monitors simultaneously. Stream multiple screens to Tesla's web browser as well as any WebRTC-compatible browser. Use tablets like iPad for an even wider workspace.

## v1.4.1 (2026-02-24)

- macOS 15 (Sequoia) support

## v1.4.0 (2026-02-22)

### New Features
- **Touch Control** — Control your macOS directly by touching the Tesla Display. Tap, scroll, and interact with your Mac through the Tesla browser screen.

## v1.3.1 (2026-02-20)

- Minor bug fixes

## v1.1.0 (2026-02-14)

### New Features
- **PIN Protection** — Optional 4-digit PIN to prevent unauthorized access on shared networks. When enabled, browsers must enter the correct PIN before streaming starts.
- **Wi-Fi Network Support** — Now displays the access IP address when connected to a regular Wi-Fi router, not just Internet Sharing. Works on any network.
- **Configurable Port** — HTTP server port can be changed from the default (80) to avoid conflicts with other services.

## v1.0.5 (2026-02-14)

- Minor bug fixes

## v1.0.4 (2026-02-13)

- Stability improvements

## v1.0.1 (2026-02-13)

- Minor fix

## v1.0.0 (2026-02-13)

- First stable release

## v0.10.7 (2026-02-13)

- Add update check and download feature

## v0.10.6 (2026-02-13)

- Stability improvements

## v0.10.5 (2026-02-13)

Initial release.
