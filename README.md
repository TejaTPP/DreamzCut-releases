<p align="center">
  <img src="dreamzcut-tile.png" alt="DreamzCut" width="100" />
</p>

<h1 align="center">DreamzCut</h1>
<p align="center">A free video editor that runs entirely on your machine.</p>

This repository holds what DreamzCut downloads and what people download to
install it. It has no source code.

- **[Releases](https://github.com/TejaTPP/DreamzCut-releases/releases)**: the
  installers for every platform (`DreamzCut-<version>-…`), a `SHA256SUMS`
  file, and the `manifest.json` the app's updater reads.
- **`models-v1`**: the AI models (captions, voices, cutout) the app fetches
  on demand, mirrored from the projects that publish them.
- **Issues**: report a problem with DreamzCut here.

Website: [dreamzcut.thedreamz.co.in](https://dreamzcut.thedreamz.co.in)

## Updates

DreamzCut looks for a newer release here when it opens, and says so in a
notice. **Settings › Version** installs it, or any earlier release from
0.1.0 on. The check can be turned off on the same page.

## Privacy and code signing

DreamzCut reaches the network only for these:

- **The update check at launch** asks GitHub for the list of releases in
  this repository once each time the app opens. It sends nothing about you;
  turn it off under **Settings › Version** with **Check for updates at
  launch**.
- **Settings › Version** asks for the same list when you open it or press
  **Check for updates**, and installing a release downloads it from here.
- **Downloading a model** fetches it from this repository's `models-v1`
  release, or from the source chosen under **Downloads** in Settings ›
  General.

Nothing is sent about you, your projects or your media, and there is no
telemetry.

The Windows builds are not code-signed yet, so SmartScreen asks before the
installer runs: **More info** › **Run anyway**. The macOS builds are not
notarised yet: if macOS will not open the app, run
`xattr -dr com.apple.quarantine /Applications/DreamzCut.app`.

## Licence

DreamzCut is free software under the GNU Affero General Public License,
version 3 or later. It is a modified version of
[Concat](https://github.com/jub0t/Concat) by Jareer Abdullah and the Concat
contributors, and is not affiliated with or endorsed by that project.

To receive the source code of any DreamzCut release, email
[tejatpp1@gmail.com](mailto:tejatpp1@gmail.com).
