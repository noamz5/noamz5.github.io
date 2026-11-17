# noamz5.github.io

Public homepage and privacy policy for **Permits Archiver**, a private Telegram bot
that copies the photos and documents (delivery permits) posted in one Telegram
group into a Google Drive folder.

The site is published with GitHub Pages at <https://noamz5.github.io/>.

## Why this site exists

The bot uploads to Google Drive using a Google sign-in (OAuth). Google only lets
such an app be set to **In production** if its OAuth consent screen links to a
**homepage** and a **privacy policy** on a domain the owner controls. Without
that, the app stays in *Testing* mode and Google cancels the bot's sign-in every
7 days. These two pages meet that requirement. The bot itself never reads them.

## Files

| File | Published at | Purpose |
|---|---|---|
| `index.html` | <https://noamz5.github.io/> | Homepage. Explains what the bot does and does not do. Used as **Application home page** on the Google consent screen. |
| `privacy.html` | <https://noamz5.github.io/privacy.html> | Privacy policy: what is stored (photos, documents, sender name, date, caption), where (the operator's Google Drive), the limited `drive.file` access, Google's *Limited Use* statement, and how to ask for removal. Used as **Application privacy policy link**. |
| `README.md` | (this file) | Explains the repository. |

## Where these values are used

Google Cloud Console → *Google Auth Platform* → **Branding**:

| Field | Value |
|---|---|
| Application home page | `https://noamz5.github.io/` |
| Application privacy policy link | `https://noamz5.github.io/privacy.html` |
| Authorized domains | `noamz5.github.io` |

## Editing

- The source copies of both pages live in the bot's project under `docs/`. Edit
  them there, then upload them here (*Add file → Upload files*). GitHub Pages
  republishes within about a minute.
- If the bot's behaviour changes, update `privacy.html` and its *Last updated* date.
- Keep this repository limited to these public pages. It is public: never add the
  bot's code, settings, tokens or credentials here.
