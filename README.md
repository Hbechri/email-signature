# Hatim BECHRI — Email Signature

`install-outlook.html` is the only production signature file.

## Design

The signature is assembled from lossless slices cropped directly from the approved
design `reference/signature-reference.png` (1620 × 540 px source, displayed at
540 × 180 px). The slices live in `assets/final-slices/` and are reassembled in a
nested, email-safe HTML table — no positioning, transforms, media queries, or
duplicate versions. Several slices are wrapped in links so the social icons,
university logos, emails, and names stay independently clickable.

The slices are hosted with [jsDelivr](https://cdn.jsdelivr.net/gh/Hbechri/email-signature@main/assets/final-slices/)
from the [Hbechri/email-signature](https://github.com/Hbechri/email-signature)
repository (`main` branch). The images must stay publicly hosted, otherwise the
signature will not render in mail clients.

## Install in Outlook

1. Open the hosted `install-outlook.html` page in **Microsoft Edge**.
2. Select the whole signature and copy it.
3. In Outlook (**Settings → Mail → Signatures**) paste it into a new signature and set it as default.
4. Do **not** edit individual elements after pasting — the layout is a single sliced image group.

## Test

Send yourself a test email and confirm in **Outlook** and **Gmail** that every slice
loads, there are no seams, and all social, mailto, and university links work.
