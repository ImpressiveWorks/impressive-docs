---
title: Alerts and failover
summary: What happens when emails keep failing.
group: Mail
order: 6
---

## When an email fails

The email is marked as failed in the [email log](log.md), with the error message.

> [!WARNING] Failed emails are not re-sent
> Impressive Mail does not re-send a failed email automatically.

## Failure alerts

If emails keep failing, the site admin gets an email alert. By default, this happens after 3 failures in a row.

Alerts are rate-limited, so you are not flooded.

Impressive Mail Pro can also send alerts to Slack, Discord, Microsoft Teams, Telegram and SMS.

## Failover to another connection

You can add more than one connection. If a connection fails 5 times in a row, Impressive Mail stops using it for 10 minutes. It sends new emails through your next active connection.

![Connection A sends your email. After 5 failed emails in a row, A is paused for 10 minutes and new emails go to Connection B, your next active connection. The admin gets an email alert, by default after 3 failures in a row. The failed emails are not re-sent.](images/failover.png "What happens when a connection keeps failing.")

To add a second connection, see [Add a connection](connections.md).
