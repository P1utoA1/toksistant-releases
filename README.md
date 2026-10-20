# Toksistant

**Your TikTok. Your terms.** An independent TikTok Account Management Assistant in OLED black, silver, and liquid glass.

## Use Toksistant

- [Open the website](https://p1utoa1.github.io/toksistant-releases/)
- [Download the Windows x64 portable app](https://github.com/P1utoA1/toksistant-releases/releases/latest)
- [Report a problem](https://github.com/P1utoA1/toksistant-releases/issues)

## v0.1.0 — Assisted preview

Import an extracted TikTok JSON export locally. Filter following, likes, saved videos, and sounds by exact date or range. Protect mutuals using your followers snapshot. Preview and approve manual review lists, track your own results, and export history.

**This release does not automatically unfollow accounts, unlike videos, or remove favorites.** TikTok's [published API scopes](https://developers.tiktok.com/docs/en/tiktok-api-scopes) do not provide these actions. Open each item in TikTok to make the change, then record the result in Toksistant. Task statuses are self-reported.

Official login is pending TikTok developer approval and an owner-configured HTTPS backend. Login alone cannot grant bulk action permissions. This public website and offline desktop release use local import mode. See [Login Kit requirements](https://developers.tiktok.com/docs/en/login-kit-web).

## Quick start

1. In TikTok, request your account data in **JSON** format using Download your data.
2. Extract the ZIP and import the JSON file (up to 50 MB).
3. Set a date rule. **Before January 1, 2026** keeps all activity dated January 1, 2026 and later.
4. Confirm a complete followers list to preserve mutuals, or explicitly turn protection off.
5. Select matches, review the list, and make changes yourself in TikTok.

The same features are available on the website and in the Windows app. A sample workspace lets you explore without importing your data. Sample records are fictional.

## Windows download

Download the portable EXE from Releases and run it. Windows 10/11 x64. This early-access build is unsigned. Verify its SHA-256 using the release's SHA256SUMS.txt:

```powershell
Get-FileHash -Algorithm SHA256 .\Toksistant-0.1.0-Windows-x64.exe
```

## Privacy

Imported records stay on your device. No passwords, TikTok cookies, analytics, or import uploads. Browser persistence is off by default; enabling Remember workspace stores records and tasks in unencrypted local browser storage. Clear them in Privacy & settings. Exported history files remain where you save them. External TikTok and GitHub links use their own services. GitHub receives ordinary hosting requests for this website.

Followers and following dates come from a potentially outdated export. Missing dates are excluded from date-based rules. Always check current account information before making changes. Importing a new file replaces the current workspace and task history.

## About this repository

Public distribution hub: release binaries, checksums, documentation, and compiled website assets only. Implementation source is maintained privately. Compiled client code remains inspectable by browsers and desktop app users. Toksistant is not affiliated with or endorsed by TikTok. This early-access preview is provided as-is. Please never attach account exports or credentials to public issues.
