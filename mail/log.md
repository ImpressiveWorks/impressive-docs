---
title: Read the email log
summary: Search, filter and open every email sent through wp_mail(). The log is free.
group: Mail
order: 5
---

Every email sent through `wp_mail()` is logged with its status. Find the log in **Mail Ops › Emails**.

## Statuses

| Status | What it means |
| --- | --- |
| Sent | Your provider accepted the email. |
| Failed | Sending did not work. The log shows the error message. |

Delivered and bounced statuses need delivery webhooks from your provider. They are part of Impressive Mail Pro.

![Your site calls wp_mail(). Impressive Mail logs every email and passes it to your email provider. The result is Sent, or Failed with the error message saved. Delivered and Bounced need delivery webhooks from your provider, in Pro.](images/log-statuses.png "Every email gets a status in the log.")

## Find an email

- Search by subject, recipient or sender.
- Filter by date, connection and status.

![The email log in Mail Ops › Emails, with its status tabs. The search, status and connection filters are circled.](images/log-filters.png "Search and filter the log.")

## Open an email

Open any email to see its recipients, headers, attachment names and error message.

![An opened email that failed: its date, recipient, From address, subject and connection (Brevo). The error message, 550 5.1.1 The email account that you tried to reach does not exist, is circled.](images/log-detail.png "A failed email shows the error message from the server.")

## What the log stores

For each email, the log stores:

- the recipients (To)
- the From address
- the subject
- the status (sent or failed) and the date
- the error message, if sending failed
- the email headers (these can include CC and BCC addresses)
- the file names and paths of attachments (not the files)

It does not store the email body.

## How long logs are kept

You choose a number between 1 and 30 days in **Mail Ops › Settings**. The default is 30 days. Logs older than that are deleted automatically once a day.

![The Data retention settings: Log retention days is set to 30 and circled. Enable Automatic Cleanup is switched on.](images/log-retention.png "Choose how many days to keep logs in Mail Ops › Settings.")

If you turn off automatic deletion, logs are kept until you delete them. You can delete single log entries in **Mail Ops › Emails**.

Impressive Mail Pro can keep logs longer.

To keep a copy of your logs, see [Export your logs](export.md).
