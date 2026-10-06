# casa-backup — backup with proof of restore

| | |
|---|---|
| **Sector** | Agents, infrastructure and tooling |
| **Source code** | private repository — read access on request |

## What it is

A backup system for two Macs to cloud storage, using restic over rclone, and treated as an operations problem rather than a copy script. It has 22 executables in `bin/`: per-machine setup, backups split by criticality, media archiving outside restic, a browsable mirror, launchd agent installation, verification, restore with list/search/extract/mount, and a `provar` ("prove") script that genuinely tests restoration instead of just counting files. The 256-bit key is generated and stored in the Keychain without anyone typing or pasting it, and the documentation is explicit about the consequence: the Keychain dies with the Mac, and a restic repository without its password is just encrypted junk. It includes a custom secret scanner in Python, an incident report, a lessons-learned log and a restore runbook. It also treats the expiry of the storage plan as a risk with a fixed date.

---

[← back to index](../README.md)
