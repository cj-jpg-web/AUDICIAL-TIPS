# Updating AUDICIAL TIPS

Live site: https://cj-jpg-web.github.io/AUDICIAL-TIPS/

Edit `content.json` on GitHub, then Commit changes to main. Pages republishes automatically. Only repository editors can publish changes; students can read the site without accounts. You can also ask ChatGPT to update this repository.

## Announcement
Replace the empty announcements array with entries like this (sample only):

```json
"announcements": [
  {
    "date": "2026-10-24",
    "label": "Practice",
    "title": "Your announcement title",
    "body": "Your message to the team.",
    "url": "https://example.com"
  }
]
```

The url field is optional. Add newest entries first. Use actual dates and schedules only when confirmed. Set announcements back to [] to clear the board.

## Tips
Each tip has id, category, title, body, and practice fields. Copy an existing entry, use a unique id, and change the text. Categories become filter buttons automatically. Update the top-level updated date.

## Resources and examples
Add entries to resources with title, description, and url. These may link to image examples, reference websites, videos, and shared documents. Only http and https links are displayed. Keep shared document permissions accessible to the intended audience. For an image hosted here, upload it to an assets folder and use its full published Pages URL as the resource link.

Keep JSON valid: use double quotes, commas between entries, and no trailing comma after the last entry. GitHub preserves version history, so changes can be restored. The site is public; avoid publishing private student data.

## Local preview
Run `python -m http.server 8000` in this folder, then open http://localhost:8000. Open through a server rather than double-clicking index.html, since content is loaded from content.json.
