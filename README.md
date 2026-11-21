# RAMN Signer

An iPhone-first, static web app for preparing an IPA and handing it to ESign through the iOS share sheet.

## Deploy
This is a static site. Enable GitHub Pages for the `main` branch, root folder. The app will be available at `https://hoodblaqo.github.io/ramn-signer/`.

## Important limitation
iOS app sandboxing prevents a Safari website from reading ESign's private certificate storage. RAMN Signer does not extract certificates, upload files, or perform code signing. It uses the Web Share API to offer the selected IPA to installed apps that support receiving shared files. If ESign does not appear in the share sheet, open the IPA from Files and use its Share / Open In flow, or import it directly in ESign.

All file selection and sharing is initiated on-device. No backend or analytics are included.
