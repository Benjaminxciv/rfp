# Bisector App Announcements

This repo hosts the remote announcements configuration for the **Bisector** app by Reliance Fiber & Power.

#3 How It Works

The Bisector app fetches `announcements.json` from this repo on every launch. Updates you make here will appear in the app within 24 hours (or immediately for users who reinstall/clear cache).

---

## ✏️ Editing Announcements

Edit the `announcements.json` file directly on GitHub:

1. Click on `announcements.json`
2. Click the ✏️ pencil icon (top right)
3. Make your changes
4. Click **"Commit changes"**

That's it! 🎉

---

## 📄 JSON Format

```json
{
  "announcements": [
    {
      "icon": "star.fill",
      "color": "yellow",
      "title": "Your Title Here",
      "body": "Your description text goes here.",
      "tag": "NEW"
    }
  ]
}
```

### Fields

| Field | Required | Description |
|-------|----------|-------------|
| `icon` | ✅ | SF Symbol name (see below) |
| `color` | ✅ | Color name (see below) |
| `title` | ✅ | Bold headline text |
| `body` | ✅ | Description paragraph |
| `tag` | ❌ | Optional badge like `"NEW"`, `"EVENT"`, `"URGENT"` |

---

## 🎨 Available Colors

| Color | Name | Best For |
|-------|------|----------|
| 🟡 | `yellow` | New features, highlights |
| 🔵 | `blue` | Events, informational |
| 🟠 | `orange` | Updates, announcements |
| 🔴 | `red` | Urgent, warnings |
| 🟢 | `green` | Success, completed |
| 🟣 | `purple` | Special, premium |
| 🩷 | `pink` | Fun, casual |
| ⚪ | `white` | Neutral |
| 🩶 | `gray` | Low priority |

---

## 🔣 Available Icons

Icons use Apple's **SF Symbols**. Here are some recommended ones:

### 📣 Announcements & News
| Icon | Name |
|------|------|
| ⭐ | `star.fill` |
| 📢 | `megaphone.fill` |
| 📰 | `newspaper.fill` |
| 🔔 | `bell.fill` |
| 💬 | `bubble.left.fill` |
| 📌 | `pin.fill` |

### 📅 Events & Dates
| Icon | Name |
|------|------|
| 📅 | `calendar` |
| ✅ | `calendar.badge.checkmark` |
| 🕐 | `clock.fill` |
| 🎉 | `party.popper.fill` |

### ⚠️ Alerts & Status
| Icon | Name |
|------|------|
| ⚠️ | `exclamationmark.triangle.fill` |
| ℹ️ | `info.circle.fill` |
| ✓ | `checkmark.circle.fill` |
| ✗ | `xmark.circle.fill` |
| 🛠️ | `wrench.fill` |

### 🏢 Business & Work
| Icon | Name |
|------|------|
| 🏢 | `building.2.fill` |
| 👤 | `person.fill` |
| 👥 | `person.2.fill` |
| 📍 | `mappin.circle.fill` |
| 📦 | `shippingbox.fill` |
| 📈 | `chart.line.uptrend.xyaxis` |

### 💡 Features & Tips
| Icon | Name |
|------|------|
| 💡 | `lightbulb.fill` |
| 🎁 | `gift.fill` |
| ⚡ | `bolt.fill` |
| 🔧 | `gearshape.fill` |
| 🚀 | `paperplane.fill` |

> 🔍 **Browse all icons:** Open the **SF Symbols** app on Mac, or visit [sfsymbols.com](https://sfsymbols.com)

---

## 📝 Examples

### New Feature
```json
{
  "icon": "star.fill",
  "color": "yellow",
  "title": "Multi-Point Capture — Now Live",
  "body": "Capture multiple bearings in a single session. Update to the latest version to try it out!",
  "tag": "NEW"
}
```

### Upcoming Event
```json
{
  "icon": "calendar.badge.checkmark",
  "color": "blue",
  "title": "Field Training · Jul 20 2026",
  "body": "Hands-on training at RFP HQ. Register through the company portal by July 15.",
  "tag": "EVENT"
}
```

### Urgent Notice
```json
{
  "icon": "exclamationmark.triangle.fill",
  "color": "red",
  "title": "Service Maintenance Tonight",
  "body": "Systems will be offline from 11 PM - 2 AM EST for scheduled maintenance.",
  "tag": "URGENT"
}
```

### General Announcement (no tag)
```json
{
  "icon": "megaphone.fill",
  "color": "orange",
  "title": "Q3 Regional Expansion",
  "body": "RFP is extending service coverage to three new regions this quarter."
}
```

---

## ⚡ Tips

- **Keep it short** — Titles under 40 characters, body under 100 characters
- **3 announcements max**
- **Remove old announcements** — Delete events after they pass
- **Test your JSON** — Use [jsonlint.com](https://jsonlint.com) to validate before committing

---
