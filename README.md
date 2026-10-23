# Cymatic

Downloads for the Cymatic macOS app. The source repository is private; this
repository only holds release downloads.

## Install

1. Download the latest `.dmg` from **Releases**.
2. Open it and drag **Cymatic** to **Applications**.
3. The app is not notarized by Apple, so the first launch needs one extra
   step:
   - **macOS 14:** Control-click Cymatic, choose **Open**, then **Open**.
   - **macOS 15 or later:** double-click Cymatic, then open **System Settings →
     Privacy & Security**, scroll to **Security**, and choose **Open Anyway**.
   - **Terminal alternative:** `xattr -dr com.apple.quarantine /Applications/Cymatic.app`
4. Cymatic requires macOS 14 or later. Release names carry the architecture;
   the current builds are for Apple Silicon.

Each release includes a `.sha256` file. Verify a download with:

```sh
shasum -a 256 -c Cymatic-<version>-<arch>.dmg.sha256
```

The app is available under MIT OR Apache-2.0. No source is published here.
