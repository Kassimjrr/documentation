---
title: Direct replies
lang: en-US
---

# Direct replies

From your email inbox, you can directly reply to the person who submitted the form.

![Direct replies](../.vuepress/public/direct-replies.png)

To activate this feature, create an input with any of the following names:

- `mail`
- `email`
- `_replyto`
- `_email.replyto`

```html
<input type="email" name="mail" placeholder="your@email.example" />
```

```html
<input type="email" name="email" placeholder="your@email.example" />
```

```html
<input type="text" name="_replyto" placeholder="your@email.example" />
```

```html
<input type="text" name="_email.replyto" placeholder="your@email.example" />
```

::: warning
Input names starting with an underscore will be hidden from the dashboard and notification emails.
:::
