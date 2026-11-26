# Tanken components

Downloads for [Tanken](https://github.com/SeraphofNineball), a file manager for Windows.

Some Tanken features need extra programs. Instead of shipping them in the installer, Tanken downloads them from this repository's [releases](../../releases) the first time a feature needs one. You don't need to download anything here by hand: use **Settings → Data & storage → Helper programs** in Tanken.

| Component | What it's for |
|---|---|
| FFmpeg | Plays MKV, AVI, FLV, WMV and other videos in the preview pane and Quick View |
| ExifTool | Thumbnails and previews of camera RAW photos |
| NAStree scanner | The scanner behind Disk Usage |

Tanken only installs the exact files it expects: each release asset's SHA-256 fingerprint is built into the app, and a download that doesn't match is discarded before it's unpacked.

## Licenses and source code

This repository holds no source code of its own; it redistributes the programs above, unmodified.

- **FFmpeg** is licensed under the GNU GPL version 3. Each release's notes, and `SOURCE.txt` inside the FFmpeg zip, link the exact FFmpeg source commit and the [BtbN/FFmpeg-Builds](https://github.com/BtbN/FFmpeg-Builds) scripts that pin every linked library. The license text is in [`notices/ffmpeg/COPYING.GPLv3.txt`](notices/ffmpeg/COPYING.GPLv3.txt). If a source link stops working, [open an issue](../../issues) and the source will be provided, for at least three years from the release it came with.
- **ExifTool** by Phil Harvey ([exiftool.org](https://exiftool.org/)) is distributed under the same terms as Perl. Its license, and those of the Strawberry Perl runtime it ships with, are inside its zip.
- **NAStree scanner** is built from [SeraphofNineball/nastree](https://github.com/SeraphofNineball/nastree).
