---
title: Questions and answers
summary: Short answers to the questions people ask most.
group: Reference
order: 12
---

## Is the email log really free?

Yes. The free plugin logs every email and keeps the logs for up to 30 days. Impressive Mail Pro can keep them longer. See [Read the email log](log.md).

## Does the log store the email content?

No. The log stores the recipients, From address, subject, status, error message, headers and attachment file names. It does not store the email body or the attachment files.

## How long are logs kept?

You choose a number between 1 and 30 days in **Mail Ops › Settings**. The default is 30 days. Logs older than that are deleted automatically once a day. If you turn off automatic deletion, logs are kept until you delete them.

## Does it work with Gmail?

Yes. Gmail and Google Workspace connect through SMTP (`smtp.gmail.com`). You need your Gmail address and an App Password. You create the App Password in your Google Account, under Security and 2-Step Verification.

## Does it work with WooCommerce and form plugins?

Yes. Impressive Mail handles every email sent through `wp_mail()`. WooCommerce, Contact Form 7, WPForms and Gravity Forms all use `wp_mail()`.

## Can I use more than one email provider?

Yes. You can add several connections. [Smart Routing rules](routing.md) (the "Email Rules" tab on the Connections page) decide which connection sends which email. Other connections also act as backups when one connection keeps failing.

## What happens when an email fails?

The email is marked as failed in the log, with the error message. It is not re-sent automatically. If emails keep failing, the site admin gets an email alert. If one connection fails 5 times in a row, the plugin stops using it for 10 minutes and uses your next active connection. See [Alerts and failover](failover.md).

## Which statuses does the log show?

The free plugin shows "sent" and "failed". "Sent" means your provider accepted the email. Delivered and bounced statuses need delivery webhooks from your provider, which are part of Impressive Mail Pro.

## Can I switch from another SMTP plugin?

Yes. Deactivate your old SMTP plugin, then add your connection in **Mail Ops › Connections**. Only one plugin should send your site's email at a time. See [Switch from another SMTP plugin](switch.md).

## Does Impressive Mail send my data to you?

No. Your email logs stay in your WordPress database. The plugin does not send usage data anywhere. Your emails go only to the email service you set up. See [The 27 email services](services.md).

## Is there a Pro version?

Yes. Impressive Mail Pro adds longer log retention, open and click tracking, reports, delivery webhooks, alerts to Slack, Discord, Microsoft Teams, Telegram and SMS, and white-label for agencies. The free plugin has no sending limits and does not need Pro.

## Where can I get help?

Please post in the [WordPress.org support forum](https://wordpress.org/support/plugin/impressive-mail/).
