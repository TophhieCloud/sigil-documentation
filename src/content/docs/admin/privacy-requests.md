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

## The two tabs

Privacy requests has two tabs:

- **Look up** finds one person, shows what Sigil holds about them, and lets you
  export it, download a report for them, or erase it.
- **Erasure requests** lists every erasure in your organisation and answers
  whether a given address was erased.

## Look someone up

1. Open Privacy requests in the portal sidebar, under Organisation.
2. On the Look up tab, enter the person's email address.
3. Choose Look up.

You can also start from a person. On [Users and roles](/admin/users-and-roles/),
and on the Mailboxes tab of [Activity](/monitoring/activity/), each row has a
Privacy button that opens the Look up tab and looks that person up straight
away. The address never appears in the page's web address.

Every look-up is recorded in your [change log](/monitoring/change-log/), so
there is a record each time somebody looks a person up, even if they don't go on
to export or erase anything.

### The person's header

The result starts with the address you looked up and:

- **Activity**: "Active, sent a signature" and how long ago, if they sent one in
  the last 30 days. Otherwise "No signature in the last 30 days".
- **Portal role**: the role they hold in your organisation, or "No portal role".
- **Other addresses**: shown when Sigil matched more than the address you
  typed, such as an alias or the address they had before a rename. Choose it to
  see the list.

### What Sigil holds

The What Sigil holds table has a row for each kind of record Sigil has about
the person, with four columns:

- **What**: the kind of record, such as Portal access, Profile values, Signature
  requests or Survey ratings.
- **Records**: how many Sigil holds.
- **Kept for**: how long Sigil keeps that kind of record. For example, signature
  requests are kept for 90 days and survey ratings for 13 months.
- **On erasure**: what erasing the person does to that row. Each row reads one
  of:
  - **Deleted**: the records go.
  - **Name replaced with a reference**: the record stays, but the person's
    address is replaced with a reference such as "Erased person 7K3F9Q". Your
    change log entries work this way.
  - **Kept**: the record stays, and the row says why. Your billing contact, for
    example, stays until you change it on [Billing](/admin/billing-profile/).
  - **Listed for you to edit**: Sigil doesn't change these itself. Templates
    that contain the person's address are listed this way, and you edit them.

The table only shows the kinds that hold something. Below it, a line such as
"Nothing held in 12 other places" opens the list of kinds that hold nothing for
this person.

If Sigil holds nothing at all, the page says so. You can still export that
answer and send it to the person.

### Held elsewhere

Under the table, Held elsewhere lists records about the person that Sigil keeps
outside your organisation's data, with how long each is kept and why. If the
person signed your organisation up, accepted the data processing agreement or
is your billing contact, this includes Sigil's own billing and CRM contact
records. Ask privacy@usesigil.app about those.

## Note the request (optional)

After Held elsewhere, The request has two optional fields:

- **Your reference**: your own ticket number for the request, up to 64
  characters. Don't put an email address in it. Sigil refuses a reference that
  contains `@`.
- **Received on**: the day the request came in. It can't be after today.

When you enter a received date, the page shows the day the reply is due: one
calendar month later. A request received on 31 January is due on the last day
of February.

Sigil keeps both with the change log entry for an export or report, and with
the erasure, so you can match them to your ticket. They are never put in a web
address.

## Export someone's data

After looking a person up, you have two downloads.

**Export as JSON** downloads a file named `sigil-person-export-` followed by the
date. It holds every record the look-up counts, in full, including other
people's addresses where a record names them. It's meant for your own records.

**Download report** downloads a readable HTML file named
`sigil-privacy-report-` followed by the date, to send to the person who asked.
It contains the person's header, the table, each of their records in plain
sections, what is held elsewhere, your reference and dates if you gave them, and
the date it was made. Other people in the records are named by their role, such
as "an administrator" or "a colleague", not by their address. The file runs no
scripts and prints cleanly.

Neither file name carries the person's address, because the file stays on your
computer after the request is answered.

Each export and each report download is recorded in your change log as a
privacy request.

## Erase someone's data

Erasing is permanent. You can't undo it.

1. Look the person up.
2. Read the On erasure column, which says what happens to each row.
3. If you have a ticket number or received date, fill in The request.
4. Under Erase this person's data, at the bottom of the tab, choose Erase this
   person's data.
5. Type the person's email address to confirm.
6. Decide whether to also exclude the mailbox (see below).
7. Choose Erase permanently.
8. Sign in again when Sigil asks. Every irreversible action in the portal asks
   for a fresh sign-in.

The page shows the erasure's progress while it runs. When it finishes, it tells
you the reference your change log now uses for the person, such as
"Erased person 7K3F9Q".

Two erasures are refused. You can't erase yourself, so ask another admin. And
you can't erase your only admin, so make somebody else an admin first. The page
says so under Erase this person's data, and the button stays greyed out.

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

The On erasure column shows what stays for this person before you confirm. In
general:

Your change log keeps every entry. The person's address is replaced with a
reference such as "Erased person 7K3F9Q", so you can still see and count what
they did, but not who they were.

Records of account emails Sigil sent keep the date and the number of
recipients. The person's address is replaced.

If the person is your billing contact, billing keeps that address until you
change it on the [Billing](/admin/billing-profile/) page.

If the person signed your organisation up for Sigil, Tophhie Cloud keeps that as
part of its account records. Write to privacy@usesigil.app about it.

An assignment rule that names the person is deleted by the erasure.

Sigil doesn't change your templates. If a template contains the person's
address, it is listed for you to edit.

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

Nothing is marked as erased. On the Look up tab, the progress message says the
erasure didn't finish and offers Try again. On the Erasure requests tab, its
status reads Failed with a Retry button beside it. Either way, Sigil asks you to
sign in again first.

## Erasure requests

The Erasure requests tab lists every erasure in your organisation, with these
columns:

- **Reference**: the reference the change log uses for the erased person.
- **Requested by**: who started the erasure.
- **When (UTC)**: when it was started.
- **Status**: Waiting, Running, Done or Failed.
- **Mailbox excluded**: whether the mailbox was excluded as well.
- **Through your partner**: whether one of your partner's staff started it.
- **Your reference**: the ticket number given with the request, if any.
- **Due by**: the day the reply is due, worked out from the received date. It
  adds "(overdue)" once that day has passed and the erasure isn't done.

The list never shows the erased person's address, and it refreshes on its own
while an erasure is still going.

### Was this address erased?

To check whether somebody was erased, for example when they ask again later:

1. Open the Erasure requests tab.
2. Under Was this address erased?, type the address.
3. Choose Check.

The answer names the erasure by its reference only, and covers the person's
aliases too. It reads "Yes" with the date for a finished erasure, "Not yet"
when the erasure is still running or didn't finish, or "No" when Sigil has no
record of erasing that address in your organisation. Sigil doesn't keep the
address you type, and the box clears once it answers.

## When your partner erases someone

If a partner's Owner or Admin erases somebody in your organisation, your
administrators get an email saying who at the partner did it and the reference
the change log now uses. The email never contains the erased person's address.
See [emails Sigil sends](/admin/emails-sigil-sends/).

## In the change log

Look-ups, exports, report downloads and erasures all appear in the
[change log](/monitoring/change-log/) as a privacy request. Each entry gives the
person's reference rather than their address, so a look-up, an export and a
later erasure of the same person line up. An erasure entry also says whether
the mailbox was excluded.
