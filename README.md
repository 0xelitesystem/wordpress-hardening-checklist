# WordPress Hardening Checklist

A practical reference for making a WordPress site harder to break into and easier to recover. It covers accounts and logins, updates and plugins, file and server settings, database and backups, and transport and headers, ending in a single checklist you can run on any site.

An independent project. Not affiliated with, endorsed by, or sponsored by the WordPress Foundation or Automattic.

## The core idea

Most WordPress sites are compromised through a handful of predictable weaknesses: weak logins, outdated plugins, and missing backups. Hardening is mostly closing those known doors rather than chasing exotic threats. A site with strong logins, current and trimmed plugins, working backups, and traffic served over HTTPS has already avoided the large majority of real-world attacks.

## What is inside

- [01-accounts-and-logins.md](01-accounts-and-logins.md) the most attacked surface, and how to lock it down.
- [02-updates-and-plugins.md](02-updates-and-plugins.md) why outdated and abandoned plugins are the top risk.
- [03-file-and-server.md](03-file-and-server.md) permissions and settings that limit the damage.
- [04-database-and-backups.md](04-database-and-backups.md) protecting data and being able to recover it.
- [05-headers-and-transport.md](05-headers-and-transport.md) HTTPS and security headers in plain terms.
- [06-hardening-checklist.md](06-hardening-checklist.md) the full check in one place.

## How this fits the portfolio

This pairs with the security baseline already in the portfolio. The baseline covers general principles for a solo operator; this applies them specifically to WordPress, which is where many operators actually run their sites.

## How to use it

Start with `01` and `02`, because logins and plugins are where most real attacks succeed. Make sure `04` is true before anything else fails, because a working backup is what turns a disaster into an inconvenience. The checklist in `06` is the version to keep.

## A note on scope

This is general guidance, not a guarantee. Security is ongoing, threats change, and no checklist makes a site unbreakable. The goal is to close the common, known weaknesses and to be able to recover if something still gets through.

## More

Part of a catalog of single-file browser tools and plain-language references, all MIT licensed and dependency-free: [0xelitesystem.github.io](https://0xelitesystem.github.io/). Built by [elitesystem.ai](https://elitesystem.ai).

## License

MIT. Copyright 0xelitesystem 2026.
