---
version: "1.5"
---

Properties are what Obsidian is calling the information at the top of a note. You may also consider this metadata or "notes about the note".

If you use tags, then you already sort of understand the point of properties. In Obsidian, properties are very, very useful. As you work with properties, you'll likely want to reference the [[LYT Standards of Classification]] for our recommended best practices.

# Auto sorting properties

The [Linter Plugin](obsidian://show-plugin?id=obsidian-linter) has been implemented into this vault [to automatically sort properties](https://platers.github.io/obsidian-linter/settings/yaml-rules/#yaml-key-sort) when you save a note (this triggers every time you click away from an active note).

As of now, we are only using Linter to keep the main "related" and "created" properties in a uniform order. Here's the current list:

```
up
in
related
down
by
created
tags
```

If any of these properties exist in your note, they are moved to the top in this order, while everything else is put below (while maintaining its previous order).

To edit you can navigate through the following steps:

- Go to settings
- Go to the `Community Plugins` tab
- `Search installed plugins` for `Linter` and click the settings gear icon
- In the top right search bar, search for `YAML Key Sort`.
- Look for the tiny box on the right. (You should be able to see `up` and `collection`.)
- You can modify the list to fit your preferences; if you ever want to revert, you can copy and paste the default list above.
