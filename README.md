# Grouped — Artist Onboarding Email Drip Campaign

> **This is the first drip campaign.** Scope: artist signup → first Swap created. Future campaigns will follow; each column in the Figma flow doc is its own separate drip.

---

## 📁 File Index

| File | Email | Send Timing | Subject Line |
|------|-------|-------------|--------------|
| `E1WELCOME.html` | Email 1 | Immediately after email verification | Welcome To The Grouped Family! 👋 |
| `E2SWAPS.html` | Email 2 | +1 day | Your first swap takes less than 5 minutes |
| `E3DATAOWNERSHIP.html` | Email 3 | +2 days | Know your fans. Own your data. |
| `E4FOUNDERSTORY.html` | Email 4 | +3 days | Why we built Grouped |
| `E5SOCIALPROOF.html` | Email 5 | +3 days | The OnlySteves blueprint 👀 |
| `E6REENGAGEMENT.html` | Email 6 | +5 days | Still finding your footing? |
| `E7FINAL.html` | Email 7 | +7 days | Your fans are waiting |

> ⚠️ **Always pull files directly from this GitHub repo. Do not copy HTML from Notion — Notion mangles the code.**

---

## 🔁 Series Logic

- **Entry trigger:** Artist completes email verification
- **Exit trigger:** `swap_created` event fires — artist exits the series as soon as they create their first Swap
- **Future:** The `swap_created` exit may eventually lead into another drip rather than ending the flow entirely. Ben's ticket is scoped to this first column only. Once Brevo templates are ready, Ben can wire up the trigger from the site.

---

## 🔧 Brevo Variables

| Variable | What it maps to |
|----------|----------------|
| `{{artistName}}` | Artist's name |
| `{{alias}}` | Name of their Group |
| `{{swap_creation_url}}` | `https://app.grouped.com/swaps/create/` |
| `{{unsubscribe_url}}` | Unsubscribe link |


---

## 🎨 Design

Updated to align with GDS26R v1.0 Brand Guide (February 2026).

- **Font:** Satoshi via Fontshare — the approved system fallback. (Grouped Font is the brand display font but cannot be self-hosted in email.)
- **Colors:** `#111620` Navy · `#C48A3A` Bronze · `#F0EBE3` Warm Cream (background + light text)
- **Logo:** Navy variant on light background
- **Max width:** 600px
- **Mobile responsive:** Yes — `@media` breakpoint at 480px

### ⚠️ Needs Team Feedback
Colors and font have been updated to match the brand guide. **Team should confirm they're happy with the look before Alex builds in Brevo.** Please review and sign off on:
- Background color: `#F0EBE3` Warm Cream
- Accent: `#C48A3A` Bronze
- Font: Satoshi

---

## ✅ Pre-Launch Checklist

- [ ] Team signs off on brand guide alignment (colors + font)
- [ ] Brevo templates built by Alex
- [ ] Ben creates trigger ticket (Onboarding/Swap Drip)


