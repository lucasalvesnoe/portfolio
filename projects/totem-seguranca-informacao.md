# Information security quiz kiosk

| | |
|---|---|
| **Client** | State development bank |
| **Sector** | Finance, legal and compliance |
| **Code files** | 11 |
| **Lines of code** | 1,492 |
| **Extensions** | `.js` ×9, `.html` ×1, `.css` ×1 |
| **Source code** | not versioned on GitHub — available on request |

## What it is

Quiz and prize-wheel kiosk for a development bank's 1st Information Security Awareness Week — built to run on a free-standing unit in the lobby, with the constraints that implies. Plain HTML, CSS and JavaScript, no build step. The screen is designed at 1080x1920 portrait and scaled to any window. Each round has 4 questions, each from a different topic drawn from six, with shuffled answer options, and only 4 correct answers unlock the wheel; after 60 seconds without a touch, it returns to the attract screen on its own. It works offline through a service worker, because at an event the network goes down.

## Structure

```
assets/
css/
js/
```

---

[← back to index](../README.md)
