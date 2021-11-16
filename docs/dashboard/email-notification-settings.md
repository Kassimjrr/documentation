---
title: Email notification settings
lang: en-US
---

# Email notification settings

To manage your form's email notification settings, navigate to its `Settings` section.

- You can enable/disable email notifications for your workspace's team members.
- You can add guests to send email notifications to people outside your workspace/organization.

![Email notification settings](../.vuepress/public/email-notification-settings.png)

## Custom templates

You can customize the notification email template of a form.

Formspark custom email templates use the [Handlebars](https://handlebarsjs.com/) templating language.

```handlebars
<div style="text-align: left;">
  <strong>New submission:</strong>
  <div style="margin: 16px 0;">
    <strong>First name</strong>: {{data.firstName}}</div>
    <strong>Last name</strong>: {{data.lastName}}</div>
  </div>
</div>
```

### Custom Handlebars helpers

The following custom Handlebars helpers have been registered for you:

#### json

Stringifies a JSON object.

##### Usage

```handlebars
{{json data}}
```

##### Implementation

```javascript
Handlebars.registerHelper("json", function (context) {
  return JSON.stringify(context);
});
```
