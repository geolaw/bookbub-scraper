# Privacy Policy

`bookbub-scraper` is a personal automation script, not a public product. It is used
by a single individual (its author) to read their own Gmail inbox and repost free
ebook deals to a Facebook Page they administer.

## What it accesses

- **Gmail (read-only)**: The script searches the owner's own Gmail inbox for emails
  from BookBub, using the `gmail.readonly` OAuth scope. It only reads message
  content to extract book titles, authors, and links — it never sends, modifies,
  labels, or deletes anything in the mailbox.
- **Facebook Page**: The script posts book deals (as found in the owner's inbox) to
  a Facebook Page the owner administers, via a Page Access Token.

## What it does with that data

Extracted book information (title, author, cover image URL, and link) is processed
locally on the owner's own machine and either printed to the terminal or posted to
the owner's own Facebook Page. Nothing is transmitted to any third party, sold,
shared, or used for advertising or analytics.

## What is stored, and where

Small JSON state files (list of previously-seen book URLs, and OAuth tokens) are
stored locally on the owner's own machine, under `~/.bookbub_scraper/`. Nothing is
stored in any cloud service or third-party database controlled by this project.

## Who this applies to

This app is not intended for use by anyone other than its author. It is not
distributed, and there is no sign-up flow — the only Google account that can
authorize it is the developer's own test account.

## Contact

Questions about this script can be directed to the repository owner via GitHub:
https://github.com/geolaw/bookbub-scraper
