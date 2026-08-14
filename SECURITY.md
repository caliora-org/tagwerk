# Reporting a security or privacy problem

Do not open a public issue for it. Use
[private vulnerability reporting](../../security/advisories/new) — the report is visible to the
maintainer only, and it stays that way until there is a fix.

## What is worth reporting

tagwerk keeps notes as plain files on the device and, if sync is switched on, on a WebDAV
server the user chooses. Anything that breaks either of those assumptions is in scope:

- note content readable by another app, another user, or an unrelated server
- sync credentials leaving the keychain, being logged, or being sent in the clear
- a certificate or hostname check that does not happen
- a state in which notes are silently overwritten or destroyed by sync
- the app requesting or retaining more data than it says it does

Out of scope: the tracker itself, GitHub, and anything about caliora.org that is not tagwerk.

## What to expect

An acknowledgement within a few days, and a fix or an explanation of why there will not be one.
tagwerk is in beta and maintained by one person; there is no bounty, and no deadline other than
"as fast as it can be done". Coordinated disclosure is welcome — say when you intend to publish
and it will be worked toward.
