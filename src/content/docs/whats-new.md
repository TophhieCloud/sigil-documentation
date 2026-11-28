---
title: What's new
description: Recent changes to Sigil that admins, partners and mailbox users can see, newest first.
---

<!-- last-portal-commit: de76333 -->
<!-- last-addin-commit: 98b46f0 -->
<!-- last-flag-check: 2026-11-28T09:03:30Z -->

This page lists changes to Sigil that you can see or need to know about, newest
first. Each entry is dated by the day the change reached Sigil and links to the
page that covers it in full. Features still in testing are left off until they
are available to every organisation.

## November 2026

### 27 November

- **Usage & rebilling in two tabs.** The page now has a Daily usage tab, where
  it opens, and a Seat history tab for one client at a time. Choosing a
  client's name in the daily table opens its seat history. Export CSV is on
  the Daily usage tab. See
  [A client's seat history](/partners/billing/#a-clients-seat-history).
- **Seat history on your Billing page.** Your subscription tab now has a Seat
  history card showing, day by day, the licensed mailboxes Sigil counted, the
  prepaid mailboxes inside that count and the number you were billed for. You
  can look up any day or list the days a figure changed, over 90 days, 12
  months or all history. See [Seat history](/admin/billing/#seat-history).
- **Each client's seat history for partners.** Usage & rebilling now has a Seat
  history card for one client at a time, current or former, with seats, prepaid
  and billable seats per day from the same rows as your invoice. The Prepaid
  and Billable columns in the usage table are now always shown. See
  [A client's seat history](/partners/billing/#a-clients-seat-history).
- **The header names what you opened.** On the template editor and a tracked
  link's detail page, the header breadcrumb now ends on the template's name or
  the link's site and path, as in "Monitoring › Link clicks ›
  contoso.com/pricing", instead of a general "Editor" or "Link detail". The
  browser tab keeps the general name. See
  [Finding your way around](/start/quickstart/#finding-your-way-around).
- **The designer's preview waits for a whole address too.** The Live preview in
  the designer now re-renders once the Render as and Sent by boxes are empty or
  hold a whole address, as the HTML editor already did. While you type, the last
  preview stays on screen instead of flashing a "No such user" error. See
  [Previewing as a particular person](/signatures/previews/#previewing-as-a-particular-person).

### 26 November

- **Privacy request entries are for admins only.** Look-ups, exports, report
  downloads and erasures in the change log are now visible only to admins, and
  to a partner's Owners and Admins working in your organisation, with an
  "Admins only" badge. Those entries now name the person by email address
  until they are erased, when the address is replaced with their reference.
  See [Privacy request entries](/monitoring/change-log/#privacy-request-entries).
- **Partner billing figures as tiles.** The figures on the Your subscription tab
  now sit in a row of tiles across the top, with the pricing note and buttons
  beneath. Seats in use also shows how many clients it counts, as in "across 12
  clients". See
  [Partner billing](/partners/billing/#checking-the-period-so-far).
- **Add-ons in the partner estimate.** "This month, estimated" on Partner
  billing now includes add-ons such as a branded link domain, not just seats.
  When add-ons are part of it, a line below splits the figure into seats and
  add-ons, so a partner whose mailboxes are all prepaid can see the add-on
  charge before the invoice arrives. See
  [Partner billing](/partners/billing/#checking-the-period-so-far).
- **Partner billing in tabs.** The Partner billing page is now split into
  Your subscription, Seats by client, Billing details and Documents, and a "!"
  marks a tab that needs you, such as a missing card or incomplete invoice
  details. The open tab stays in the address bar, so paying an invoice brings
  you back to Documents. See
  [Partner billing](/partners/billing/#the-partner-billing-page).
- **A breadcrumb in the header, and pages sized to fit.** The portal header now
  shows where you are, such as "Organisation › Billing", and on a detail page it
  links back to the list, as in "Monitoring › Link clicks › Link detail". On a
  large monitor each page keeps to a centred column, narrower for forms and
  settings and wider for tables, logs and the template editor. See
  [Finding your way around](/start/quickstart/#finding-your-way-around).
- **Who manages your account, out of the way.** If a partner manages your
  organisation, the Managed by notice has moved from the top of every page to a
  chip in the sidebar, and removing their access is now on a Partner access card
  in Settings, on the tab now called Partner & support access. The audit log has
  a Made by filter for changes from your organisation, your provider or Sigil
  support. See [Partner access](/admin/settings/#partner-access).
- **A readable privacy report, and request tracking.** Privacy requests now has
  Look up and Erasure requests tabs. After a look-up you can download a
  readable report to send the person, which names other people by their role
  instead of their address, and note your ticket reference and the day the
  request came in so the page shows when the reply is due. The Erasure requests
  tab lists every erasure with its due date and can tell you whether an address
  was erased. See [Privacy requests](/admin/privacy-requests/#erasure-requests).
- **Each row says what erasure does to it.** The look-up's table now gives, for
  each kind of record, how many Sigil holds, how long it is kept, and whether
  erasing deletes it, replaces the name with a reference, keeps it or lists it
  for you to edit. Every look-up is now recorded in your change log. See
  [What Sigil holds](/admin/privacy-requests/#what-sigil-holds).
- **Privacy requests in the portal.** Admins, and a partner's Owners and Admins
  working in a client, can now look a person up by email address, see what
  Sigil holds about them, export it as a JSON file, or erase it. Erasing asks
  you to type the address and sign in again, and can also exclude the mailbox
  so Sigil stops creating new data about it. Users and roles and the Activity
  Mailboxes tab have a Privacy button that opens the page for that person. See
  [Privacy requests](/admin/privacy-requests/).
- **Erased people keep their change log entries under a reference.** After an
  erasure, the change log keeps every entry the person made but shows a
  reference such as "Erased person 7K3F9Q" instead of their address. If a
  partner does the erasure, your administrators get an email with that
  reference. See
  [Who each entry names](/monitoring/change-log/#who-each-entry-names).
- **Names last only as long as access.** Sigil now keeps a person's name only
  from their sign-in token, and only while they have portal access. Once their
  access ends, the change log shows their address alone. See
  [Who each entry names](/monitoring/change-log/#who-each-entry-names).
- **Billing details need every required field to save.** Save billing details
  now stays greyed out until the legal company name, billing email, address
  line 1, city, postcode and country are all filled in, and the form names any
  that are missing. This applies on Billing, Partner billing and the getting
  started checklist. See
  [When it counts as complete](/admin/billing-profile/#when-it-counts-as-complete).

### 25 November

- **Deletion grace window is now 29 days.** When your organisation is scheduled
  for deletion, the purge now runs no more than 29 days later rather than 30, so
  your data is gone within the 30 days the data processing agreement allows. The
  first deletion email names the day. See
  [Deleting your data](/security/data-and-privacy/#deleting-your-data).
- **Recycle bin covers templates only.** The privacy policy's retention table
  now says that only a deleted template sits in Recently deleted for 30 days. A
  deleted footer, banner or image is removed straight away and cannot be
  brought back. See
  [Retention](/security/compliance/#retention).

### 24 November

- **Photo retention stated correctly.** The privacy policy's retention table now
  says a profile photo is cached for up to seven days after it was last read
  from Microsoft 365, refreshed once the copy is a day old. It previously said
  24 hours. See
  [Retention](/security/compliance/#retention).

- **Privacy policy names the global caches.** The privacy policy, updated on 24
  November 2026, now says plainly that short-lived cached copies of rendered
  signatures, and of the directory details they are built from, can sit on
  Cloudflare's network outside the UK and EEA. They expire on their own. The data
  processing agreement has not changed. See
  [Where data lives](/security/data-and-privacy/#where-data-lives).

- **Taking a mailbox off the cost list by API.** Scripts that use an API key now
  remove a mailbox from the cost management list with
  `POST /api/admin/exclusions/remove`, naming it in the body as
  `{ "email": "..." }`. The old `DELETE /api/admin/exclusions/:email` path now
  answers 404, so update any script that calls it. See
  [Organisation endpoints](/reference/api/#organisation-endpoints).

### 23 November

- **Format a field chip from the toolbar.** Selecting a field chip in a text
  block now keeps the toolbar up, and bold, italic, underline, colour, link and
  clear formatting apply to that chip. Ctrl+B, Ctrl+I and Ctrl+U work on it too,
  and the chip's settings gain Italic and Underline beside Bold. See
  [Formatting a field chip](/signatures/designer/#formatting-a-field-chip).
- **Build a design from the keyboard.** Clicking a tile on the Blocks rail, or
  pressing Enter on it, adds the block after the selected one without dragging.
  Tab selects blocks on the canvas, and Alt+Up and Alt+Down arrow move the
  selected block one place. Dialogs keep Tab inside them and return you to
  where you were when they close. See
  [Working without a mouse](/signatures/designer/#working-without-a-mouse).
- **A live preview that doesn't flash.** The designer's live preview keeps the
  last render on screen until the next one is ready, so it no longer goes blank
  while you type. See [The live preview](/signatures/designer/#the-live-preview).
- **Save a design before it's finished.** The designer now saves a draft while
  blocks are still waiting for content, such as an image block with no image
  picked or a button with no link. The message says how many things are left,
  and the draft can't be submitted for review or published until they are done.
  See
  [Saving a design you haven't finished](/signatures/designer/#saving-a-design-you-havent-finished).
- **Your images on the canvas.** Library images and uploaded social icons now
  show as the real picture in the designer, and Browse lets you pick one from
  thumbnails. The inspector shows an image's natural size, with Use it to apply
  it, and Keep proportions keeps width and height in step. A file over 1 MB
  is turned away before it uploads. See
  [Referencing an image](/signatures/images/#referencing-an-image).
- **Pick a font and a background for the signature.** Signature settings now
  offer a list of email-safe fonts, with Custom stack… for your own, and a
  Background colour for the whole signature. See
  [Canvas settings](/signatures/designer/#canvas-settings).
- **The designer points you at each problem in turn.** Choosing the things to
  finish or dark-mode risks chip beneath the canvas now steps through each
  problem and says what it is, instead of going back to the first one every
  time. The text toolbar now sits in a bar above the stage, clear of the blocks.
  See [Finding each problem](/signatures/designer/#finding-each-problem).
- **The designer asks before it publishes.** Publish, Staged and Approve and
  publish now ask you to confirm first, as they already did in the HTML editor,
  and the buttons are unavailable while a change is still being saved. With a
  saved draft and unsaved edits, Discard asks whether to throw away only the
  edits or the draft as well. See
  [Discarding a draft](/signatures/publishing/#discarding-a-draft).
- **Copy, paste and duplicate blocks from the keyboard.** In the designer,
  Ctrl+D duplicates the selected block, and Ctrl+C and Ctrl+V copy a block and
  paste it after the one you select. Duplicating now selects the copy. A field
  chip you click is selected on its own, and Delete removes it. See
  [Copying, pasting and duplicating blocks](/signatures/designer/#copying-pasting-and-duplicating-blocks).
- **Undo in the designer goes back one thing at a time.** Dragging a colour
  across the picker is now one undo step, and pausing, leaving a control or
  selecting something else starts a new one. Ctrl+Z inside a text block undoes
  the design, not only your typing, and Ctrl+Y redoes. Undo and Redo are greyed
  out when there is nothing to undo or redo. See
  [Undo and redo](/signatures/designer/#undo-and-redo).
- **Enter and spaces in the designer do what you typed.** Pressing Enter in a
  text block starts a new line, and that line break is in the signature people
  send. Doubled spaces and spaces at the start or end of a line
  now survive in the signature people receive. See
  [Line breaks and spacing](/signatures/designer/#line-breaks-and-spacing).
- **Links in the designer can be edited and removed in place.** Put the cursor
  in a link and choose the link button to change its address, or remove the
  link and keep the text, its colour and its visibility rule. Links on the
  canvas now show in the canvas link colour, and hovering shows where they go.
  See [Links in a text block](/signatures/designer/#links-in-a-text-block).
- **The add-in reuses its token between messages.** On Outlook on the web, new
  Outlook, Mac and mobile, the add-in now keeps an encrypted copy of the token it
  uses to fetch your signature, so the next message doesn't wait for Outlook to
  issue a new one. It is never kept for a shared mailbox, and is discarded five
  minutes before it expires. See
  [The copy kept on the device](/security/data-and-privacy/#the-copy-kept-on-the-device).

### 19 November

- **The signature log shows more on each row.** Each row now names the
  template the signature came from, whether it was the new message or reply
  signature, and the Outlook it ran in. An arrow at the end of a row opens the
  rest of the event, including the HTTP status, duration and request ID. See
  [Reading a signature log row](/monitoring/activity/#reading-a-signature-log-row).
- **Activity is now split into tabs.** Activity has Overview, Mailboxes and
  Signature log tabs. Each row in the By
  mailbox table has a Log button that opens the Signature log tab already
  searched for that mailbox. See
  [What the view shows](/monitoring/activity/#what-the-view-shows).
- **Previewing as a person waits for a whole address.** In the HTML editor, the
  preview now re-renders once the address box holds a whole address, typed in
  full or picked from the suggestions. A half-typed name no longer brings up a
  "No such user" error while you type. See
  [Previewing as a particular person](/signatures/previews/#previewing-as-a-particular-person).

### 18 November

- **Settings is now split into tabs.** Settings has General, Emails, Link
  domain and Support access tabs, laid out like Billing. The tab is part of the
  page address, and the link in the health digest now opens the Emails tab. See
  [Settings](/admin/settings/).
- **Let Sigil support make changes for a set time.** Settings has a new Sigil
  support access switch. An admin can let support change your templates,
  banners, footers, rules and profile fields for 1 to 24 hours, and switching it
  off ends their session at once. It is off unless you turn it on. See
  [Sigil support access](/admin/settings/#sigil-support-access).
- **See why support is in your portal.** Support now gives a reason every time
  they open your portal, read-only or not. The reason appears in your change
  log, and the Settings page lists the support sessions open right now. See
  [Seeing who is in your portal](/admin/settings/#seeing-who-is-in-your-portal).

### 17 November

- **One grace period per departure from a partner.** An organisation that
  leaves a partner again within 30 days of its last grace period starting, or
  within the grace period's length if that is longer, now keeps the deadline it
  already had to add a card instead of getting a new grace period.
  See [The grace period after leaving](/partners/clients/#the-grace-period-after-leaving).
- **A listed alias now counts its mailbox in.** In inclusion mode, a mailbox
  whose alias is on the list, rather than its primary address, is now billed as
  a seat and appears on the Billed mailboxes tab. Before, sends from that alias
  got a signature but the mailbox was not counted. See
  [What reads the other way round](/admin/cost-management/#what-reads-the-other-way-round).

### 16 November

- **See which mailboxes you are billed for.** Cost management has a new Billed
  mailboxes tab that lists every mailbox counting towards your seats, by name,
  with a filter and a CSV download. The Billing view links to it from the seat
  figure. See [Seeing who is billed](/admin/cost-management/#seeing-who-is-billed).
- **Cost management is split into tabs.** The page now has Excluded mailboxes,
  Groups, Billed mailboxes and Mode tabs, and a tab that needs attention carries
  a ! marker. See [The page's tabs](/admin/cost-management/#the-pages-tabs).

### 14 November

- **A disabled Sigil app now sends the reconnect email.** If an admin turns off
  Sigil's enterprise application in Entra, or deletes it, the nightly check now
  treats it like withdrawn consent and emails your administrators "Action
  needed: reconnect Sigil". A disabled application needs switching back on in
  Entra, which granting consent again does not do. See
  [Consent has lapsed](/deploy/connect-your-organisation/#consent-has-lapsed).

### 12 November

- **The change log records more of what happens to your account.** Cancelling
  or reactivating from Billing, saving invoice details, saving a card, partner
  management requests and their answers, and a mailbox's signature download now
  each leave an entry. For invoice details, the entry names the fields that
  changed, not their values. See [Change log](/monitoring/change-log/).
- **Support actions carry an operator reference.** Entries made by Tophhie Cloud
  support now read "Sigil operator" with a short reference such as `OP-7K3F`.
  The same person always has the same reference, so you can tell their actions
  apart and quote one to support without being told who they are. See
  [Actions taken by Tophhie Cloud support](/monitoring/change-log/#actions-taken-by-tophhie-cloud-support).

### 10 November

- **Tracked links keep every query parameter.** A tracked link whose destination
  had more than one query parameter used to drop everything after the first.
  Sigil now keeps them all. Links in mail you have already sent are repaired
  too, so nobody needs to resend anything. See [Link clicks](/monitoring/link-clicks/).
- **Roles you give are limited by your own.** Someone who manages users without
  being an admin can only give a role that holds no more than their own, so
  Billing can no longer make another account an Editor. The invite dialog now
  opens on a role you're allowed to give. See [Users and roles](/admin/users-and-roles/).
- **A trial's first charge has no grace period.** If the first payment after a
  free trial fails, signatures pause straight away rather than after the usual
  grace period, and the first email you get says so. See [Billing](/admin/billing/).
- **Contact cards carry only what your signature shows.** A contact card now
  holds your name and address plus the fields your signature itself prints.
  Contact card links made before the change keep company, job title and business
  phone. See [Contact card](/signatures/contact-card/).
- **Partners can't release a client that has no admin.** Releasing a client is
  refused until the client has an admin of its own, so nobody unexpected becomes
  its admin by signing in first. See [Clients](/partners/clients/).

### 9 November

- **Choose the day your health digest arrives.** Admins can now pick the day
  the health digest is sent, and weekly and monthly digests each keep their own
  choice. A monthly digest no longer drifts earlier each month. Settings shows
  when the last digest went out and when the next one is due.
- **The digest covers the time since the last one.** Its published and feedback
  sections now run from the previous digest rather than a fixed seven days. Your
  organisation's first digest covers seven days and waits for your chosen day
  instead of going out at once. See [Health digest](/monitoring/health-digest/).

### 4 November

- **Sigil's emails follow dark mode.** The emails Sigil sends you now switch to
  a dark card when your mail app is in dark mode, and keep a clear edge in light
  mode. See [Emails Sigil sends](/admin/emails-sigil-sends/).

### 3 November

- **A new look for the portal.** The portal and Sigil's own emails use a new
  plum colour scheme, and the portal sits in a framed layout.

## October 2026

### 30 October

- **Plain-text paste and a formatting eraser in the designer.** Text you paste
  into the designer arrives as plain text, without formatting from wherever you
  copied it. A new eraser clears the formatting from highlighted text. See
  [Designer](/signatures/designer/).
- **A letterhead layout for Sigil's emails.** The account and billing emails
  Sigil sends now use a letterhead-style layout. See
  [Emails Sigil sends](/admin/emails-sigil-sends/).

### 29 October

- **Links keep their font size in Outlook.** A link inside a text block sometimes
  showed smaller than the text around it in Outlook. The designer now carries
  the block's font size onto every part of the text, links included. See
  [Designer](/signatures/designer/).

### 27 October

- **Reactivating a cancelled subscription works first time.** Reactivate no
  longer keeps failing after you save a card, and any discount you agreed now
  applies to the first invoice too. If the card is refused, the message tells
  you to add a card and try again. See [Billing](/admin/billing/).

### 26 October

- **Sigil emails you when your account changes.** You now get an email when your
  service or billing changes, including when a colleague or Tophhie Cloud
  changes what you pay. Whoever pays the bill is told, not only the person who
  made the change. Sigil also warns you a week before an API key expires. See
  [Emails Sigil sends](/admin/emails-sigil-sends/).
- **The people an action affects are told about it.** A draft's author hears
  when it is published or sent back, with the reviewer's note. Other admins hear
  when someone gains or loses admin access, and when a restore replaces later
  edits. A new organisation's first admin gets a welcome email with the trial's
  end date. See [Emails Sigil sends](/admin/emails-sigil-sends/).
- **Changes to the legal agreements reach every organisation.** A change to the
  Data Processing Agreement or the Partner Agreement is sent to every
  organisation as a service notice, which product update opt-outs don't stop.
  Adding or replacing a sub-processor carries 30 days' notice. See
  [Compliance](/security/compliance/).
- **Partners get the notices the Partner Agreement promises.** Partners are
  emailed about suspension, removal, the end of a partnership, reactivation and
  a returned client. Suspension and removal emails give the reason and the date
  they take effect. See
  [How you are told](/partners/leaving-the-programme/#how-you-are-told).
- **A lapsed client request no longer blocks the next one.** When a request to
  manage a client, or an invitation, lapses unanswered, it stops showing as
  pending and you can send another. The partner's owners and admins, and whoever
  sent it, are emailed when it lapses. See [Clients](/partners/clients/).

### 25 October

- **Prepaid blocks are confirmed by email.** When Tophhie Cloud records a
  prepaid block of mailboxes, or ends one early, whoever pays for it is emailed.
  For a partner-paid block the email names the client. See
  [Prepaid mailboxes](/admin/billing/#prepaid-mailboxes).

### 23 October

- **Partners covered by prepaid blocks aren't asked for a card.** The partner
  warning about a missing card now counts seats after any prepaid blocks, so a
  partner whose clients are all covered no longer sees it. A live branded link
  domain still needs a card, and the warning names the domains. See
  [Partner billing](/partners/billing/).

### 21 October

- **Your signature shows the moment the pane opens.** The Sigil pane in Outlook
  now shows the signature it kept from last time straight away, then checks for
  a newer one. See [My signature pane](/users/my-signature-pane/).
- **A faster portal.** Pages now load their panels only when you open them,
  card payment forms load on demand, and your browser keeps the portal's files
  between visits.
- **The change log loads a page at a time.** Long change logs now open quickly
  and offer a Load more button for older entries. See
  [Change log](/monitoring/change-log/).
- **Billing counts seats nightly.** The Billing page shows the seat count taken
  in the previous night's directory scan, and says which day it was counted,
  instead of counting every time the page opens. See [Billing](/admin/billing/).

### 19 October

- **Turn the compliance footer off for a template.** A template can now leave
  out your organisation's compliance footer. Whoever turns it off has to
  acknowledge what that means first, and the change is recorded in the change
  log. See [Footers](/targeting/footers/).

### 14 October

- **Keep campaign banners off a template.** A template can now opt out of
  campaign banners, so its signature never carries one while a campaign runs.
  See [Keeping banners off a signature](/targeting/banners/#keeping-banners-off-a-signature).

### 9 October

- **Preview, edit and test any banner.** Every banner, not only the live one,
  now has Edit and Preview, and can be sent to you as a test. The test email
  gains a banner choice, and the designer's live preview has a banner date
  picker so you can see what a signature will carry on a given day. See
  [Banners](/targeting/banners/).

### 6 October

- **Custom roles.** Admins can define their own roles in Users and roles, with
  a name, a description and the areas of the portal each one reaches. Custom
  roles appear wherever a role is chosen, and invite emails describe them. See
  [Users and roles](/admin/users-and-roles/).
- **Prepaid mailboxes.** A block of mailboxes bought up front now shows on the
  Billing page, and billing charges only for mailboxes above it. Partners see
  it on Partner billing, in Usage and in the usage export. See
  [Prepaid mailboxes](/admin/billing/#prepaid-mailboxes).

### 5 October

- **A clearer start to the free trial.** The trial sign-in screen now states the
  trial terms, links the permissions Sigil asks for, and gives a setup link you
  can pass to your IT admin. The Getting started checklist puts a working
  signature first and billing after it. See
  [Starting from the free trial](/deploy/connect-your-organisation/#starting-from-the-free-trial)
  and [Getting started checklist](/admin/getting-started-checklist/).

### 4 October

- **Deploy the add-in from the Microsoft Marketplace.** Sigil's Outlook add-in
  is listed in the Microsoft Marketplace, and the Getting started checklist now
  sends you there instead of asking you to upload a manifest. See
  [Deploy the add-in](/deploy/deploy-the-add-in/).

### 1 October

- **Pay without leaving the portal.** Adding a card now opens a payment form
  inside the portal instead of sending you to a separate checkout page, and an
  open invoice can be paid from the Documents tab. See [Billing](/admin/billing/)
  and [Invoices and credits](/admin/invoices-and-credits/).
- **Partner bills follow the average number of mailboxes.** Partners are billed
  on the average of daily mailbox counts across the period, rather than the
  count on its last day. Each partner moves over at its first billing period
  starting on or after 1 October, and the invoice explains the figure. See
  [Partner billing](/partners/billing/).

## September 2026

### 28 September

- **Live updates, and seeing who else is editing.** The portal and the designer
  now update as colleagues make changes. When someone else has the same template
  open, the editor says so. When they save a draft, you're told and can reload
  to see it, rather than having what you typed replaced. See [Publishing](/signatures/publishing/).

### 25 September

- **Prices exclude VAT.** Prices are now shown excluding VAT, and VAT is added to
  invoices where it applies. See [Billing](/admin/billing/).
- **Payment failure emails say what the bank said.** When a card payment fails,
  the email gives the bank's reason, names the card, and tells you what to do
  about that particular reason. See [Emails Sigil sends](/admin/emails-sigil-sends/).
- **Saves no longer overwrite a colleague's change.** If someone else changed a
  template since you opened it, your save is refused and your text is kept, so
  nothing is lost silently. Booking a schedule or starting a rollout over an
  existing one now asks you to confirm the replacement. See
  [Publishing](/signatures/publishing/).

### 24 September

- **Pictures of your signatures.** Each published version, and each draft sent
  for approval, now has a picture of the signature filled in for a sample
  person. Pictures appear in the template library, in version history, in the
  approval email and in the health digest. See [Previews](/signatures/previews/).
- **Ask the documentation.** A question box in the portal answers from this
  documentation and links the pages it used. See
  [Ask the documentation](/admin/ask-the-documentation/).
- **Combine conditions with and, or and not.** The designer's "Show when"
  setting opens a rules dialog where conditions can be grouped and combined.
  The HTML editor accepts the same logic. See [Designer](/signatures/designer/)
  and [HTML editor](/signatures/html-editor/).
- **The digest names who published.** Each template listed as published in the
  health digest now shows who published it. See
  [Health digest](/monitoring/health-digest/).

### 22 September

- **Branded link domains.** A new paid add-on lets tracked links in signatures
  use your own domain instead of Sigil's. You set it up in Settings, where the
  DNS record to add is shown for you to copy, and buy or drop it from Billing. See
  [Branded link domain](/monitoring/branded-link-domain/).
- **Partners can add the link domain for clients.** Partners can turn the
  branded link domain on for a client from Clients, and it is billed on the
  partner's invoice. See [Partner billing](/partners/billing/).
- **A paused mailbox isn't asked again for ten minutes.** When Sigil refuses a
  mailbox's signature, for example because delivery is paused, the add-in notes
  it on that device and waits ten minutes before asking again. After you resume
  delivery, signatures can take up to ten minutes to come back on a device. See
  [Pausing delivery](/signatures/pausing-delivery/).

### 16 September

- **Images and backups are stored in the EU.** Uploaded images and backups are
  now kept in Cloudflare's EU jurisdiction. See
  [Infrastructure](/security/infrastructure/).

### 15 September

- **Every directory attribute for the sender.** The sender fields now cover
  company, address, office, fax and the manager's name, job title, email and
  phone. See [Placeholders](/signatures/placeholders/).
- **Rules on part of a text block.** In the designer, you can highlight some
  text and give just that text its own rule, so it only shows when the rule
  matches. See [Designer](/signatures/designer/).
- **Logos keep their shape on phones.** Images in a signature now keep their
  proportions when a mail app narrows them to fit a small screen. Outlook for
  Android used to squash wide logos. See [Images](/signatures/images/).
- **More time for a first signature.** The first message from a mailbox, or from
  a device with no saved copy, now waits up to fifteen seconds for its signature
  instead of five, so fewer go out unsigned. See [Activity](/monitoring/activity/).
- **One more Microsoft address to allow.** Outlook's own runtime loads part of
  itself from `ajax.aspnetcdn.com`. If your network limits outbound addresses,
  allow it. See [Requirements](/deploy/requirements/).
- **Product update emails, with an off switch.** Admins can receive occasional
  emails about what has changed in Sigil. A switch in Settings stops them for
  the whole organisation, and each email has its own opt-out link. See
  [Settings](/admin/settings/).

### 13 September

- **Start a template from your website.** The New template dialog can read your
  logo, brand colour, address and social profiles from your public website. You
  check what it found before anything is created. See
  [Templates](/signatures/templates/).
- **Check your own signature is working.** The page for mailbox users shows
  whether Sigil last added your signature to an email, and the reason if it
  didn't. See [Your details](/users/your-details/#whether-your-signature-is-working).
- **Limits on image uploads.** Each image can be up to 1 MB, as PNG or JPEG.
  The Images page shows how many images and how much storage your organisation
  has used. See [Images](/signatures/images/) and [Limits](/reference/limits/).
- **Signature request records are kept for 90 days.** Records of individual
  signature requests and their outcomes are now deleted after 90 days. Summaries
  per mailbox and daily totals are kept while you use Sigil. See
  [Activity](/monitoring/activity/).
- **Billing details are needed before a trial converts.** A trial only becomes
  a paid subscription once your billing details are complete. Without them, the
  trial ends on its date and nothing is charged. The checklist asks for billing
  details before the payment method. See [Billing details](/admin/billing-profile/).
- **Billing is split into tabs.** The Billing page now has tabs for your
  subscription, billing details, documents and the DPA. A tab that needs
  something from you is marked. See [Billing](/admin/billing/).

### 10 September

- **Sender profile fields.** Templates can use the sender's own profile answers
  with `{{sender.custom.<key>}}`, for mail sent from a shared or delegated
  mailbox. See [Profile fields](/admin/profile-fields/).
- **Fill in profile fields for any mailbox.** Admins can add answers for a
  mailbox nobody has filled in yet, such as a shared mailbox, with Add mailbox.
  See [Profile fields](/admin/profile-fields/).

### 9 September

- **Shared mailboxes added as an account.** Sigil now works in a shared mailbox
  added as a full account in new Outlook for Windows, or opened in its own tab
  in Outlook on the web. See [Deploy the add-in](/deploy/deploy-the-add-in/).
- **See which add-in version each mailbox has.** Activity shows the add-in
  version each mailbox installed, and a notice appears when mailboxes are behind.
  See [Activity](/monitoring/activity/).
- **An audit log page of its own.** The change log moved to its own page under
  Monitoring, with filters, a CSV export and a detail view of what changed. See
  [Change log](/monitoring/change-log/).
- **People shown by name.** Across the portal, people are shown by their current
  name alongside their email address. See [Users and roles](/admin/users-and-roles/).
- **The pane's preview fits the pane.** The preview in the Sigil pane is laid out
  at the pane's own width, so text wraps rather than the whole signature being
  shrunk. See [My signature pane](/users/my-signature-pane/).

### 8 September

- **Microsoft 365 group mailboxes.** Signatures can now be targeted at mail sent
  from a group mailbox, with conditions for sent from a group mailbox and not
  sent from one. See [Group mailboxes](/signatures/group-mailboxes/).
- **Rules save as you go.** Adding, editing, removing or reordering an assignment
  rule is saved straight away. See [Assignment rules](/targeting/assignment-rules/).
- **Signatures appear faster in Outlook.** The add-in applies the signature it
  kept from the mailbox's last message at once, then checks it against the
  current one. The first message after a publish can show the old signature
  before it switches. See [Publishing](/signatures/publishing/).

### 7 September

- **A feedback board.** Help and the support page now link to the feedback board
  at `feedback.tophhie.cloud`. See [Troubleshooting](/deploy/troubleshooting/).
- **Preview an old version before restoring it.** Archived versions can be
  previewed with sample details before you restore one. See
  [Versions](/signatures/versions/).

### 6 September

- **Aliases are matched to the mailbox.** An alias typed into the exclusion or
  inclusion list is now matched to the mailbox's main address. See
  [Cost management](/admin/cost-management/).

### 5 September

- **Three ways to start a template.** The New template dialog offers a starter
  signature, a blank canvas or the HTML editor. See
  [Templates](/signatures/templates/).
- **Service status in the portal.** The portal header shows the service status,
  read from Sigil's status page. See [Infrastructure](/security/infrastructure/).
- **Include mailboxes instead of excluding them.** Cost management has an
  inclusion mode, where only the mailboxes you list get signatures and are
  billed. See [Cost management](/admin/cost-management/).
- **A sample person from a fictitious company.** The starter template and the
  sample person in previews now use Contoso, a fictitious company. See
  [Templates](/signatures/templates/).

### 4 September

- **Pay by invoice, and account credits.** Accounts can be set up to pay by
  invoice, and the Billing page lists your invoices with credits and credit
  notes beside them. See [Invoices and credits](/admin/invoices-and-credits/).
- **Bank transfers shown on Billing.** Money received by bank transfer but not
  yet applied to an invoice now shows on the Billing page. See
  [Invoices and credits](/admin/invoices-and-credits/).
- **Free arrangements with an end date.** A partner's client list shows "Free
  until" and the date when a client's free arrangement runs to a date. See
  [Clients](/partners/clients/).

### 3 September

- **Cancelling runs to the end of the paid period.** A cancelled subscription
  keeps working until the period you've paid for ends. A banner says when
  signatures aren't being served for a billing reason. See
  [Cancelling](/admin/billing/#cancelling).
- **A billing warning on every page.** People who can open Billing see a banner
  when a trial is in its last week with no card, or a failed payment is counting
  down to the date signatures stop. See [Billing](/admin/billing/).
- **A prompt to accept the DPA.** Admins see a prompt at the top of the portal
  when the Data Processing Agreement hasn't been accepted, or a newer version is
  out. See [Compliance](/security/compliance/).
- **Footer fixes.** A blank footer can no longer be saved, a leading @ on the
  domain is accepted, and editing a paused footer keeps it paused. See
  [Footers](/targeting/footers/).

### 2 September

- **Dark mode in the designer's preview.** The live preview can show a signature
  the way Outlook and Gmail recolour it in dark mode, and warns about text that
  could become hard to read. See [Dark mode](/signatures/dark-mode/).
- **Mailbox and Sender fields side by side.** The designer's field menu is split
  into Mailbox and Sender, so you choose whose details a field shows. See
  [Designer](/signatures/designer/).
- **No Google Fonts needed.** The portal, the designer and the Outlook pane now
  serve their own fonts, so Google's font hosts don't need to be reachable. See
  [Requirements](/deploy/requirements/).

### 1 September

- **Pause signatures for the whole organisation.** Delivery can be paused and
  resumed from the Templates page. See [Pausing delivery](/signatures/pausing-delivery/).
- **Help inside the portal.** A Help button opens links to the documentation and
  your support contact. For a managed organisation, that contact is its partner.
  See [Troubleshooting](/deploy/troubleshooting/).
- **Trial and payment reminders.** Sigil emails you three days and one day before
  your trial ends, and tells you when a payment fails. Partners' billing contacts
  are emailed when a partner payment fails, with the date clients' signatures
  would stop. See [Emails Sigil sends](/admin/emails-sigil-sends/).
- **Works behind data loss prevention proxies.** The add-in now sends the
  mailbox address in the body of its request rather than in the web address,
  which some data loss prevention tools blocked.
- **Clearer errors in the pane.** The Sigil pane now tells a problem at Sigil's
  end apart from not being able to reach Sigil at all. See
  [Troubleshooting](/deploy/troubleshooting/).

## August 2026

### 30 August

- **Per-client detail on partner invoices.** Partner invoices list seats for
  each client, and Usage lists the periods already invoiced. See
  [Partner billing](/partners/billing/).
- **Support actions show in your change log.** Anything Tophhie Cloud support
  does to your organisation now appears in your change log as a Sigil operator.
  See [Change log](/monitoring/change-log/).
- **Partner Agreement revised.** The revised agreement adds breach notification
  within 24 hours, the terms for leaving the programme, and 90 days' notice
  before the programme closes. Partners accept the new version. See
  [Partner Agreement](/partners/agreement/) and
  [Leaving the programme](/partners/leaving-the-programme/).

### 29 August

- **Signatures for shared mailboxes and sending on behalf.** Templates can tell
  a send from your own mailbox apart from one sent from a shared mailbox or on
  someone's behalf, and show the sender's details. See
  [Sending on behalf](/signatures/sending-on-behalf/).

### 22 August

- **An uptime commitment for partners.** The Partner Agreement commits to 99.9%
  monthly uptime with service credits, and sets out how support is split
  between partners and Tophhie Cloud. See [Service level](/partners/service-level/).

### 19 August

- **Enter adds a new line in dialogs.** Pressing Enter in a dialog's text editor,
  such as the footer's, now starts a new line instead of saving the dialog.

### 12 August

- **Sigil is provided by Tophhie Cloud Ltd.** The legal documents and Sigil's
  emails now name Tophhie Cloud Ltd, its company number and registered address.
  See [Compliance](/security/compliance/).
