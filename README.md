# Narly Properties

A free, offline property management app for UK landlords. Everything runs in your web browser and nothing is sent to a server.

**Open the app: https://chf-4u.github.io/narly-properties/**

## What it records

| Area | What you can keep |
|---|---|
| **Properties** | Address, nation, type, council tax band, mortgage and fixed-rate end date, keys, notes |
| **Compliance** | Gas Safety (CP12), EICR, EPC (warns below E), smoke/CO alarms, landlord insurance, legionella, HMO and selective licences, landlord registration, boiler service, PAT, fire risk, and more. Each one has its expiry date, result and the certificate PDF |
| **Viewings** | Enquiries and viewings, and where each applicant came from. You can turn an applicant into a tenant with one click |
| **Tenants** | Contact details, referencing result, Right to Rent check and follow-up date, guarantor, emergency contact, forwarding address |
| **Tenancies** | Rent and frequency, holding deposit, deposit scheme, protection date and prescribed information, rent review date, notice and termination details, deposit return |
| **Move-in checklist** | 21 steps, from viewing through referencing, deposit protection, documents given, inventory, meter readings and keys |
| **Move-out checklist** | 13 steps, from notice through check-out, final readings, keys and deposit return |
| **Inspections** | Check-in, routine, alarm test and check-out, with damp/mould flag and next-due date |
| **Repairs** | Priority, contractor, quote and cost, status |
| **Utilities and meters** | Suppliers, account numbers, who pays, MPAN/MPRN, meter readings with photos |
| **Money** | Rent received, rent account and arrears for each tenancy, expenses, and a tax-year (6 April to 5 April) summary with CSV export |
| **Tasks, contacts, documents** | Reminders, contractors (Gas Safe numbers and so on), and every attachment in one place |
| **Dashboard** | One list of everything that needs attention, plus a compliance grid of all properties |
| **Calendar** | Exports an `.ics` file of every expiry and deadline, with alerts 30 days and 7 days before. It works with Google, Outlook and Apple Calendar |

## How to use it

### On a computer (Windows, Mac or Linux)
Double-click `index.html`. It opens in Chrome, Edge, Firefox or Safari. Keep the app folder somewhere safe, such as Documents, and bookmark the page.

### On a phone or tablet, installed like an app (free)
Phones can't easily open local files, so put the folder on free static hosting:

1. Create a free GitHub account, make a new repository, and upload the 4 files (`index.html`, `manifest.webmanifest`, `sw.js`, `icon.svg`).
2. Open the repository's **Settings → Pages**, choose **Deploy from branch → main**, and save.
3. Open the web address it gives you on your phone. Then:
   - **iPhone:** in Safari, tap Share → **Add to Home Screen**.
   - **Android:** in Chrome, tap ⋮ → **Install app**.

The app then works offline. The web address only holds the app itself; your data stays on each device.

## 🔒 Login (optional, free)

Go to **Backup & settings → Login & security → Turn on login** and choose a username and password. Once it's on:

- The app asks for your password each time it opens. It also locks itself after a period of no activity (15 minutes by default, which you can change), and there's a **🔒 Lock** button in the top bar.
- Your records and attached documents are **encrypted on the device** (AES-256), using the encryption built into your browser. Without the password, nobody can read them, even with access to the computer.
- Backups are encrypted with the same password.
- **If you forget your password, your data can't be recovered.** Keep a backup and write the password down somewhere safe. If you're locked out, you can erase the device from the sign-in screen and restore a backup, as long as you remember the password that was in use when you made it.

Login applies to each device. On a second device, restore your backup there and then turn login on.

## ⚠️ Backups: your data lives on one device

Data is saved inside the browser on the device you use. To keep it safe:

- Go to **Backup & settings → Download full backup** regularly. The backup includes all your attached files. The dashboard reminds you after 30 days without one.
- Save the backup file to a USB stick or a free cloud drive (OneDrive, Google Drive or iCloud).
- To move to another device, download a backup on the old one, open the app on the new one, and choose **Restore**.
- Clearing your browser's "site data" deletes the app's data. Don't use private or incognito windows.

## Notes
- The built-in **UK landlord guide** page is a memory aid, not legal advice. Rules differ between England, Wales, Scotland and Northern Ireland, and they change, including the Renters' Rights Act roll-out in England. Check gov.uk before you act.
- There's no bank connection by design. You record rent and costs by hand.
- It's built with plain HTML, CSS and JavaScript only: no frameworks, no accounts and no cost.
