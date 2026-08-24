# email-assets

Public static assets referenced from Smallest.ai email signatures.

| File | Use |
|---|---|
| `smallest-logo.png` | Signature mark, 128x128, whitespace trimmed, displayed at 56px |
| `smallest-logo-original.jpg` | The original supplied file, 454x430, kept for reference |
| `apoorv-sood.jpg` | Signature headshot, 256x256, displayed at 56px |
| `devansh-pawan.png` | Signature headshot, background removed, 256x256, displayed at 56px |
| `akshat-mandloi.png` | Signature headshot, background removed, 256x256, displayed at 56px |

These files are public because email clients fetch signature images over
plain HTTPS with no credentials. Do not put anything non-public here.
Renaming or deleting any of these will break the image in every signature that has
already been sent. The logo files are no longer referenced by the signatures but are
kept in case we switch back.

Serve these over **GitHub Pages** (`https://vaibhavmehta277.github.io/email-assets/...`),
never `raw.githubusercontent.com`. Raw URLs carry
`content-security-policy: default-src 'none'; sandbox` and `x-frame-options: deny`, which makes
some mail clients and preview panes refuse to render the image, and they cache for only
5 minutes.
