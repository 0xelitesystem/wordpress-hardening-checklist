# Database and backups

Protect the database that holds your site's content and keep working, tested, off-site backups, because a backup you can actually restore is what turns a compromise or failure from a catastrophe into an inconvenience. If you do one thing from this reference, make it backups.

## Why backups come first

Every other measure tries to prevent a problem. Backups assume one will eventually happen anyway. Sites get hacked, hosts fail, updates break things, and people make mistakes. A current backup you can restore means none of those is the end of the site. Without one, any single failure can be permanent. This is why backups are the foundation, not an afterthought.

## What a real backup looks like

A backup worth having is recent, complete, stored away from the site itself, and proven to restore. Recent, so you lose little. Complete, meaning both files and database. Off-site, so a problem with the server does not take the backup with it. And tested, because a backup that has never been restored is only a hope. Schedule them automatically and verify restores periodically.

## Harden the database

The database holds everything: content, users, settings. Use a strong, unique database password, and where supported, change the default table prefix so automated attacks targeting the standard names are less effective. Ensure the database is not exposed to the public internet beyond what the site requires. These steps make the database a harder target and limit who can reach it.

## Keep credentials out of reach

Database credentials live in the site's configuration file, so protecting that file, as covered in the file settings, is part of protecting the database. Anyone who reads those credentials can reach the data directly. Treat the database password with the same care as any other key: unique, strong, stored safely, and never exposed in client-side code or public repositories.

## Plan the recovery, not just the backup

Know how you would actually restore the site, and roughly how long it would take, before you need to. A backup is only half of recovery; the other half is a clear path from backup to a working site. Having restored at least once, so the process is familiar, is what makes a backup genuinely protective rather than theoretically reassuring.
