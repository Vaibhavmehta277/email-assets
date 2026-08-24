# email-assets

Public static assets referenced from Smallest.ai email signatures.

| File | Use |
|---|---|
| `smallest-logo.png` | Signature mark, 128x128, whitespace trimmed, displayed at 56px |
| `smallest-logo-original.jpg` | The original supplied file, 454x430, kept for reference |

These files are public because email clients fetch signature images over
plain HTTPS with no credentials. Do not put anything non-public here.
Renaming or deleting `smallest-logo.png` will break the logo in every
signature that has already been sent.
