# Bible & Songbook

An offline Android Bible and hymn/songbook application.

## Features

- Fully offline Bible and songbook
- KJV Bible reader with book, chapter, and reference navigation
- Song search by title, number, or words
- Song categories
- Favorite songs
- Book-style left/right hymn swiping
- Persistent Bible text highlighting with selectable colors
- Notes for verses and highlighted passages
- Saved-items hub for highlights, favorite songs, and notes
- Light, dark, and system themes
- Adjustable reading text size
- No Android `INTERNET` permission

Favorites, highlights, notes, settings, and recent items are stored locally on the device.

## Privacy

The app is designed to work without network access. The Android manifest intentionally does **not**
request the `INTERNET` permission, and the WebView blocks network loads. External attribution links,
when opened by the user, are handed to the device's external browser.

## Building

Requirements:

- Android Studio
- Android SDK 35
- JDK bundled with Android Studio is suitable

Open the project directory in Android Studio and build the app.

From the Android Studio terminal on Windows, if Java is not already configured:

```powershell
$env:JAVA_HOME="C:\Program Files\Android\Android Studio\jbr"
$env:Path="$env:JAVA_HOME\bin;$env:Path"
```

Then use Android Studio's **Build > Build APK(s)** command.

For a public GitHub release, use Android Studio's **Build > Generate Signed App Bundle or APK**
and keep the signing keystore private. Never commit a `.jks` or `.keystore` file.

## Release

Public release version: **1.0.0**

Suggested Git tag: `v1.0.0`

## Attribution

App icon:

[Bible icons created by Magnific - Flaticon](https://www.flaticon.com/free-icons/bible)

## Content and licensing

The application source code is licensed under the MIT License; see `LICENSE`.

The MIT License applies to the application code only. Bundled Bible text, hymn/song text, icon
artwork, and other third-party content are **not relicensed** by this repository. Their respective
copyright, public-domain status, licenses, and attribution requirements remain with their original
sources/rightsholders.

Before redistributing bundled textual content publicly, the repository owner should verify the
redistribution status of every included hymn/song text in the intended jurisdictions.

## Security note

Do not commit signing keys, passwords, `local.properties`, IDE-local configuration, or build output.
