---
title: Install Impressive Mail
summary: Install the free plugin from WordPress.org. After you activate it, a setup wizard helps you connect your email provider.
group: Getting started
order: 1
---

## Requirements

| You need | Version |
| --- | --- |
| WordPress | 6.6 or higher |
| PHP | 8.2 or higher |

Not sure which versions you have? If you use WP-CLI, run these two commands on your server:

```bash
wp core version   # needs 6.6 or higher
php -v            # needs 8.2 or higher
```

## Install from WordPress.org

1. In your WordPress admin, go to **Plugins › Add New Plugin**.
2. Search for "Impressive Mail".
3. Click **Install Now**, then **Activate**.
4. The setup wizard opens. Follow it to connect your email provider and send a test email. See [Run the setup wizard](wizard.md).

> [!NOTE] Using another SMTP plugin?
> Deactivate it first. Only one plugin should send your site's email at a time. See [Switch from another SMTP plugin](switch.md).

## Install by hand

Upload the plugin ZIP file in **Plugins › Add New Plugin › Upload Plugin**, then activate it.

## Where to find things

You can change everything later in the **Mail Ops** menu.

| Menu | What it holds |
| --- | --- |
| Connections | Add, edit and test connections. The "Email Rules" tab holds your Smart Routing rules. |
| Emails | The email log. |
| Settings | Log retention and automatic deletion. |
| Export | Export your email logs. |
