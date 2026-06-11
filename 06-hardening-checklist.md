# Hardening checklist

The full WordPress hardening check in one place. Start with logins, plugins, and backups, since that is where most real risk and recovery live.

## Accounts and logins

- [ ] No account uses admin as its username.
- [ ] Every account has a long, unique password in a password manager.
- [ ] Two-factor authentication is enabled on all accounts that can change the site.
- [ ] Failed login attempts are limited.
- [ ] Each account has only the role it needs, and unused accounts are removed.

## Updates and plugins

- [ ] Core, themes, and plugins are current.
- [ ] Security updates are applied promptly.
- [ ] Unused plugins and themes are deleted, not just deactivated.
- [ ] Everything installed comes from a trusted, maintained source.
- [ ] What is installed is audited on a regular schedule.

## Files and server

- [ ] File permissions follow least privilege.
- [ ] The built-in theme and plugin file editor is disabled.
- [ ] The configuration file is protected and not web-readable.
- [ ] Upload directories cannot execute code.
- [ ] The site volunteers little version or error detail publicly.

## Database and backups

- [ ] Automatic backups run on a schedule.
- [ ] Backups include files and database, stored off-site.
- [ ] A restore has been tested and the recovery path is known.
- [ ] The database uses a strong, unique password.
- [ ] Database credentials are protected and never exposed.

## Headers and transport

- [ ] The entire site is served over HTTPS.
- [ ] Plain HTTP redirects to HTTPS, with a strict-transport policy set.
- [ ] Straightforward security headers are in place.
- [ ] Any content security policy has been built up and tested carefully.

## The one-line version

Strong logins with two-factor, current and trimmed plugins, tested off-site backups, and HTTPS everywhere close the doors most attacks actually use. Everything else is a useful layer on that foundation.
