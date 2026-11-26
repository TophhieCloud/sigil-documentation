---
title: Privacy requests
description: Find what Sigil holds about one person in your organisation, export it as a file, or erase it, to answer an access or erasure request.
sidebar:
  order: 8
---

When somebody asks your organisation what it holds about them, or asks for it
to be deleted, Privacy requests is where you answer for the part of it that
lives in Sigil. You look the person up by email address, see what Sigil holds
about them, and then export it, erase it, or both.

## Who can use it

Privacy requests is open to the Admin role only, along with a partner's Owners
and Admins working in an organisation they manage. The data it covers spans
users, profile fields, exclusions and monitoring, so no narrower role is the
right bar. Other roles, custom roles and [API keys](/admin/api-keys/) can't
reach it.

Tophhie Cloud support can't open it either, even during a
[support session](/admin/settings/#sigil-support-access). If you ask support to
run an export or erasure for you, they use their own tools, and the action is
recorded as theirs.

## Look someone up

1. Open Privacy requests in the portal sidebar, under Organisation.
2. Enter the person's email address.
3. Choose Look up.

You can also start from a person. On [Users and roles](/admin/users-and-roles/),
and on the Mailboxes tab of [Activity](/monitoring/activity/), each row has a
Privacy button that opens this page with their address filled in.

Sigil covers the person's other addresses as well as the one you type, such as
their aliases and the address they had before a rename.

The result lists what Sigil holds about them, as a count for each kind of
record. Depending on the person, that can include:

- their portal access
- the values they entered in [profile fields](/admin/profile-fields/)
- a mailbox [exclusion](/admin/cost-management/), and any excluded group that
  covers them
- their signature requests from the last 90 days, and the summary of their
  signature activity
- survey ratings left on their emails
- [assignment rules](/targeting/assignment-rules/) that name them
- sign-ins from before your organisation connected
- partner access to your organisation, where they work for your partner
- [change log](/monitoring/change-log/) entries they made, and entries about
  them
- account emails and notices Sigil sent them
- their name, and a cached copy of their directory record

If Sigil holds nothing, the page says so.

Below the list, a section called What erasure keeps says what would stay behind
if you erased this person, and why. It only lists the lines that apply to them.

## Export someone's data

After looking a person up, choose Export as JSON. Your browser downloads a file
named `sigil-person-export-` followed by the date. The file name never carries
the address, because the file stays on your computer after the request is
answered.

The file holds the same records the lookup counts, in full. It also lists the
templates whose content contains the person's address, and flags such as
whether they are your billing contact.

Each export is recorded in your change log as a privacy request.

## Erase someone's data

Erasing is permanent. You can't undo it.

1. Look the person up.
2. Read What erasure keeps.
3. Choose Erase this person's data.
4. Type the person's email address to confirm.
5. Decide whether to also exclude the mailbox (see below).
6. Choose Erase permanently.
7. Sign in again when Sigil asks. Every irreversible action in the portal asks
   for a fresh sign-in.

The page shows the erasure's progress while it runs. When it finishes, it tells
you the reference your change log now uses for the person, such as
"Erased person 7K3F9Q".

Two erasures are refused. You can't erase yourself, so ask another admin. And
you can't erase your only admin, so make somebody else an admin first.

### Excluding the mailbox as well

Erasing removes what Sigil holds today. It doesn't stop the person using Sigil.
If they still work for you and keep sending email from Outlook, Sigil reads
your directory for their signature again and records new activity, as it does
for anybody else.

The confirmation offers a switch, "Also exclude this mailbox, so Sigil stops
creating new data about it". It is off by default. Turn it on if the person
should stop getting a Sigil signature. Sigil then
[excludes](/admin/cost-management/) the mailbox once the erasure finishes.

If the person looks active, the confirmation warns you. That happens when they
sent a message in the last 30 days, or when they have portal access. The warning
is there to inform you and doesn't block the erasure.

If your organisation uses [cost management](/admin/cost-management/) to list the
mailboxes Sigil serves, rather than the ones it doesn't, there is no switch.
Erasing takes the person off that list, so Sigil stops providing their
signature.

### What erasure keeps

Some records have to survive, and the page says which ones apply before you
confirm.

Your change log keeps every entry. The person's address is replaced with a
reference such as "Erased person 7K3F9Q", so you can still see and count what
they did, but not who they were.

Records of account emails Sigil sent keep the date and the number of
recipients. The person's address is replaced.

If the person is your billing contact, billing keeps that address until you
change it on the [Billing](/admin/billing-profile/) page.

If the person signed your organisation up for Sigil, Tophhie Cloud keeps that as
part of its account records. Write to privacy@usesigil.app about it.

An assignment rule that names the person is deleted by the erasure. The page
names each rule first.

Sigil doesn't change your templates. If a template contains the person's
address, the page tells you how many do, and you edit them yourself.

If the person works for your partner, their partner records stay with the
partner.

A few copies expire on their own:

- Survey links and contact cards in emails they already sent stop working.
- Colleagues' cached directory records may name the person as their manager for
  up to 7 days.
- Backups expire within 30 days.
- Outlook may keep a copy of their last signature on their device for up to 45
  days.

### If an erasure doesn't finish

The status reads "Didn't finish" and nothing is marked as erased. Choose Try
again, on the progress message or beside the erasure under Past erasures. Sigil
asks you to sign in again first.

## Past erasures

The bottom of the page lists every erasure in your organisation, with its
reference, who asked for it, when, and its status: Waiting, In progress, Erased
or Didn't finish. The list never shows the erased person's address.

## When your partner erases someone

If a partner's Owner or Admin erases somebody in your organisation, your
administrators get an email saying who at the partner did it and the reference
the change log now uses. The email never contains the erased person's address.
See [emails Sigil sends](/admin/emails-sigil-sends/).

## In the change log

Exports and erasures both appear in the [change log](/monitoring/change-log/) as
a privacy request. An erasure entry gives the person's reference and says
whether the mailbox was excluded as well. An export entry gives the same
reference, so an export and a later erasure of the same person line up.
