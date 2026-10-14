# PyPocket — manual support-mail retention (90 days)

**Developer:** Ahmed Alenzi  
**Support mailbox:** pypocket.support@gmail.com  
**Approved rule:** Retain support correspondence for **90 calendar days from the date a support case closes**, unless a longer legal retention obligation applies. Requests for earlier deletion should also be handled.

This is a **manual process**, as chosen by the developer. No Google Apps Script or Gmail integration is required.

## Practical workflow

1. Keep a **private log**, outside the public GitHub repository. Suggested fields: `ticket reference | sender email | closed date | delete-on date | status | actual deletion date`. Avoid copying message bodies, attachments, access tokens or other sensitive details into the log.
2. When the support issue is resolved, send a final reply and record the actual **closed date**. Set **delete-on = closed date + 90 calendar days**. If the ticket is reopened, update its status and recalculate from its later final closure.
3. Review the log **at least once a week**. For entries past their delete-on date, search Gmail for the exact thread, confirm no ongoing case or valid legal retention requirement, delete the correspondence and any related copies you control, and record the completion date. Empty Trash when appropriate. Gmail's standard `older_than:90d` search is **not sufficient**; it uses a message's age, not the ticket closure date.
4. If someone requests earlier deletion, receive it at **pypocket.support@gmail.com**, preferably with the subject **Support Data Deletion Request** / **طلب حذف بيانات الدعم**. Confirm which correspondence is theirs (verify ownership if necessary), delete records under your control when appropriate, and respond with confirmation or explain a lawful retention restriction.
5. Keep Gmail access protected with multi-factor authentication. Never request passwords, one-time login codes or API tokens from users.

## Before publishing the revised privacy policy

- [ ] Start the private log and make sure you can record each case's closing date and delete-on date.
- [ ] Schedule a weekly reminder to review the log (or use an existing reliable routine).
- [ ] Confirm the actual app release matches the privacy statements and Google Play's Data safety declarations.

The policy's 90-day commitment applies **whether deletion is manual or automated**. This document does not itself delete email messages.
