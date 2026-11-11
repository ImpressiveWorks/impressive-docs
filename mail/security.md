---
title: Security
summary: How passwords and API keys are stored, who can change the settings, and what stays on your site.
group: Reference
order: 11
---

## Passwords and API keys

Passwords and API keys are encrypted in the database with AES-256-CTR. The key comes from your WordPress security keys, `AUTH_KEY` and `SECURE_AUTH_KEY`.

## Who can change the settings

Only administrators can see or change the settings. Admin actions are protected by WordPress nonces.

## What stays on your site

- Your email logs stay in your WordPress database. See [What the log stores](log.md#what-the-log-stores).
- The plugin does not send usage data anywhere.
- Your emails go only to the email service you set up. See [The 27 email services](services.md).

![Your WordPress site with Impressive Mail sends the email and the login details to the email service you set up, for each email and each test. Your email logs stay in your database. Nothing goes to impressive.works: no usage data.](images/data-flow.png "What leaves your site, and what stays.")
