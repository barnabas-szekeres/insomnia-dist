# insomnia-dist

Signed builds of Insomnia for Mac, the notes and tasks app. The sources are private; only what the
app downloads is published here.

- **Releases**: one per version, tagged `desktop-v<version>`, each with the `.dmg` (signed with a
  Developer ID and notarized), the update archive `Insomnia_<version>_aarch64.app.tar.gz`, its
  minisign signature (`.sig`) and `latest.json`.
- **Updates**: the app reads `releases/latest/download/latest.json` to find a new version, and
  installs only archives signed with the update key whose public half it carries.

To install, download the `.dmg` from the latest release and drag Insomnia to Applications. It runs
on Macs with Apple silicon.
