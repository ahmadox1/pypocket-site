# PyPocket support correspondence — 90-day retention procedure

**Owner:** Ahmed Alenzi  
**Mailbox:** pypocket.support@gmail.com  
**Policy:** Retain support correspondence for 90 calendar days **after closure**, except when longer retention is legally required. This runbook must be implemented operationally before publishing the revised privacy notice.

## Manual operation (no integrations required)

1. In Gmail, create labels `PyPocket/Open`, `PyPocket/Closed`, `PyPocket/Deletion-Request` and `PyPocket/Legal-Hold`. These labels organize cases; they **do not** automatically delete anything.
2. When a support request comes in, assign `PyPocket/Open`. Keep a **private** register (not in a public repository) with ticket reference, sender email, opening date, and case status. Do not put message bodies, secrets, or sensitive project files in that register.
3. When the matter is resolved, send the final response, mark the ticket closed, and record the **actual closure date** and a **deletion due date exactly 90 calendar days later**. Move the thread to `PyPocket/Closed` and remove `PyPocket/Open`.
4. Set a weekly review calendar reminder to check the private register for due tickets. For each due ticket, check any legal retention obligations or active dispute first. If there is no valid reason to retain it, delete the related support emails and attachments from the mailbox and **Empty Trash** when appropriate; consider copies/exports you control as well. Record only the completion date and ticket reference in the private register. If held, document the reason and next review date privately.
5. For an early deletion request sent to `pypocket.support@gmail.com` with subject **Support Data Deletion Request** (Arabic: **طلب حذف بيانات الدعم**), verify ownership if needed, identify all related correspondence under the developer's control, and complete the deletion or provide a clear reason for lawful retention. Record the outcome in the register; never ask for passwords, verification codes or API keys.
6. Review and process new deletion requests regularly, preferably within a few business days, and ensure the privacy notice accurately reflects actual practices.

## Do not rely on Gmail age searches alone

Queries such as `older_than:90d` compare message dates, **not the date a support ticket was closed**. A case reopened or closed much later could be deleted too early. Use the recorded *closure date* to calculate retention.

## Before publishing

- [ ] Owner sets up the labels and a private closure/deletion register.
- [ ] Owner sets up a recurring review reminder.
- [ ] Owner tests the workflow with a dummy support thread, including earlier-deletion requests.
- [ ] Owner confirms privacy statements against final APK/network/security audit and Play Console Data Safety.
- [ ] Then publish the pending privacy-policy PR.

This is an operating procedure; adding the file does not itself configure Gmail or ensure deletion.
