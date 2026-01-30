# Style Development - No Go/Docker Required

Use this folder to modify and preview page styles **without installing Go or Docker**.

## Quick Start

1. **Open the mockup** - Double-click `login-mockup.html`, `register-mockup.html` or `list-mockup.html` to open in your browser
2. **Edit styles** - Modify the `<style>` block inside the mockup file
3. **Refresh** - Press F5 in browser to see changes
4. **Apply to real app** - When done, copy the styles to `../web/public/css/site.css` or the corresponding view file

## Files

| File | Purpose |
|------|---------|
| `login-mockup.html` | Login page preview - edit `<style>` block |
| `register-mockup.html` | Register page preview - edit `<style>` block |
| `list-mockup.html` | File list page preview - edit `<style>` block |
| `../web/public/css/site.css` | Copy shared styles here for the real app |
| `../web/views/user/login.html` | Login page HTML structure |
| `../web/views/user/register.html` | Register page HTML structure |
| `../web/views/file/list.html` | File list page HTML structure (has inline styles) |

## Tips

- Styles are embedded in each mockup so they work without a server (no CORS issues)
- Form submit, API calls won't work (no backend) - use for visual/style development only
