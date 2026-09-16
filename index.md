---
title: Privacy policy — GCHHS MiyaCare Survey Values
description: Privacy policy for the GCHHS MiyaCare Survey Values browser extension.
---

# Privacy policy

**GCHHS MiyaCare Survey Values browser extension**

**Effective date:** [date]
**Applies to version:** 0.10.0
**Publisher:** Colin Robinson

---

## In short

This extension does not collect, transmit, sell or store your data. It has no
server, no analytics and no account. Everything it does happens inside your own
browser, and nothing it reads is ever sent to the publisher or to anyone else.

The only way information leaves the browser is if you press one of the copy
buttons, which places a table on your computer's clipboard so you can paste it
somewhere yourself.

---

## What the extension is

The extension adds a button to the activities view of MiyaCare, a clinical
application used by GCHHS for remote patient monitoring. Pressing the button
opens a read-only table of the patient-recorded values that MiyaCare has already
loaded into the page — blood glucose readings, insulin doses, observations and
food-diary text — arranged by date and task.

It operates only on these addresses:

- `https://miya.gchhs.alcidion.cloud`
- `https://miya-test.gchhs.alcidion.cloud`
- `https://miya-dev.gchhs.alcidion.cloud`

On every other website the extension is inactive and does nothing at all.

## What information the extension handles

While you are viewing a patient's activities in MiyaCare, the extension reads
the response that MiyaCare itself has already requested and sent to your
browser. From that response it extracts:

- Recorded clinical values, such as blood glucose readings, insulin doses,
  weight and observations
- Free-text diary entries recorded by the patient
- The date and time each entry was recorded
- The patient identifier contained in the response, used to make sure the table
  only ever shows the record you currently have open

This is identifiable health information. It is the same information already
displayed to you by MiyaCare under your own login. **The extension does not
request, unlock or obtain any data you are not already authorised to see.**

## What the extension does with it

The extracted values are held in your browser's memory for as long as the page
is open, and are used solely to draw the table on screen.

- They are **not written to disk**, to browser storage, to cookies or to
  extension storage.
- They are **discarded** when you close the tab, reload the page or navigate to
  a different patient. Values belonging to a previously viewed patient are
  deleted, not merely hidden.
- They are **never transmitted**. The extension makes no network requests of its
  own and has no destination to send anything to.

## What the extension does not do

- It does **not** collect or receive any personal information about you as a
  user of the extension.
- It does **not** use analytics, telemetry, crash reporting, advertising
  identifiers or tracking of any kind.
- It does **not** create an account, require a sign-in, or communicate with any
  server operated by the publisher. No such server exists.
- It does **not** load or execute any code from the internet. All of its code is
  contained in the installed package.
- It does **not** sell, share, rent or transfer data to any third party.
- It does **not** modify the clinical record, or write anything back to MiyaCare
  or any other system. It reads and displays only.

## The clipboard

The extension provides buttons that copy the on-screen table to your computer's
clipboard, so that it can be pasted into a spreadsheet or a clinical note.

This only happens when you deliberately press one of those buttons. Be aware
that once information is on the clipboard it is handled by your operating
system, not by this extension: on Windows it may remain in clipboard history,
and it may be synchronised to a Microsoft account if you have that feature
enabled. Treat copied clinical information the same way you would treat any
other patient information on your device, and paste it only where it belongs.

## Permissions

The extension requests **no browser permissions**. Its manifest declares no
`permissions` and no `host_permissions`, and it uses no browser extension APIs.
Its only access is a content script that runs on the three addresses listed
above.

## Data retention

None. The extension stores no data, so there is nothing retained and nothing to
request deletion of. Closing the browser tab removes everything it was holding.

## Security

The extension has no backend, no stored data and no network activity, which
removes most of the surface a privacy policy would usually need to address. Its
source code is a single readable JavaScript file distributed with the extension
and is available for inspection on request.

A technical design and security guide describing exactly how the extension
works, including its residual risks, is maintained by GCHHS Digital Health and
is available to reviewers on request.

## Children

The extension is a tool for clinical staff and is not directed at children. It
collects no information from anyone who uses it.

## Changes to this policy

If the behaviour of the extension changes in a way that affects this policy,
this page will be updated and the effective date above revised. Material changes
will be reflected in a new extension version.

## Contact

Questions about this policy, or requests to review the source code or the
technical guide:

**Colin Robinson, Digital Health**
Gold Coast Hospital and Health Service
colin.robinson@health.qld.gov.au

---

*This policy describes the behaviour of the software only. Handling of patient
information by GCHHS is governed by Queensland Health information privacy
obligations, including the Information Privacy Act 2009 (Qld) and the Hospital
and Health Boards Act 2011 (Qld).*
