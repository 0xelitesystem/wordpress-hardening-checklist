# Accounts and logins

The login screen is the most attacked part of a WordPress site, so harden it first: strong unique passwords, no default usernames, two-factor authentication, and limits on repeated login attempts. Most successful break-ins start here, which is why this is where hardening starts too.

## Kill the default and weak credentials

Never use admin as a username, and never reuse a password. Automated attacks try common usernames and leaked passwords by the thousand, and a default username paired with a weak password is the easiest possible target. Create an administrator account with a non-obvious username and a long, unique password stored in a password manager, and remove any leftover default account.

## Add two-factor authentication

Two-factor authentication requires a second proof beyond the password, so a stolen or guessed password alone does not grant access. For an administrator account, this is one of the highest-value protections available, because it defeats the credential-guessing and password-reuse attacks that account for so many compromises. Enable it for every account that can change the site.

## Limit login attempts

Without a limit, attackers can try passwords endlessly against your login screen. Limiting failed attempts, then locking out or slowing down repeated failures, stops automated guessing from grinding away indefinitely. This single measure neutralizes the brute-force attacks that hammer WordPress login pages constantly.

## Least privilege for every account

Give each account only the role it needs. Not everyone who touches the site needs administrator access; authors, editors, and contributors have narrower roles for a reason. Fewer administrator accounts means fewer keys to the whole site, so a compromised lower-privilege account cannot do as much damage. Review accounts periodically and remove ones no longer in use.

## Protect the login surface itself

Reducing exposure of the login page helps: serving it only over HTTPS so credentials are not sent in the clear, and considering measures that cut automated traffic to it. The combination of a hardened login page, strong unique credentials, two-factor authentication, and attempt limits turns the most attacked surface on the site into one of the better defended.
