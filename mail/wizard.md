---
title: Run the setup wizard
summary: The setup wizard helps you pick a provider, enter your details, set the From address and send a test email.
group: Getting started
order: 2
---

## When it opens

The setup wizard opens after you activate Impressive Mail. If you have not installed the plugin yet, start with [Install Impressive Mail](install.md).

## What it helps you do

1. Pick a provider.
2. Enter your details.
3. Set the From address.
4. Send a test email.

![Four steps in a row: pick a provider, enter your details, set the From address, send a test email.](images/wizard-steps.png "The four steps of the setup wizard. You can change all of it later in Mail Ops.")

## Before you start

Have the login details for your email service ready. Depending on the service, that is a username and password, an API key, or an access token.

- Many providers can send through their HTTP API when you enter an API key. Without a key, they send through SMTP.
- Gmail and Microsoft 365 connect through SMTP. For Gmail, you use an App Password. See [Does it work with Gmail?](faq.md#does-it-work-with-gmail)

Not sure your provider is supported? See [The 27 email services](services.md). You can also use any other SMTP server.

## After the wizard

You can change everything later in the **Mail Ops** menu. To add, edit or test a connection, go to **Mail Ops › Connections**. See [Add a connection](connections.md).
