# MONO Finance — iOS MVP

A minimal, local-first expense tracking app built with Expo / React Native.

## Run on your iPhone
1. Install Node.js (LTS) on your Mac.
2. In Terminal, navigate to this folder: `cd mono-finance-app`
3. Run `npm install`.
4. Run `npx expo start --tunnel` (or `npx expo start` on the same Wi-Fi).
5. Install **Expo Go** on your iPhone and scan the QR code using the iPhone Camera app.

## Smart Available to Spend
`max(0, min(starting balance + all recorded income - all recorded expenses - reserved obligations, monthly budget - monthly expenses))`.
If the minimum is negative, the Home screen shows how far you are over the limit.

## Important MVP limitations
- Data is saved only on this device using AsyncStorage; it is **not encrypted or backed up**. Do not use for sensitive financial identifiers.
- Currency changes only relabel amounts; they do not perform FX conversion.
- Reserved obligations are entered as a single total, not individual scheduled bills.
- All transaction dates use the current device time; dates cannot yet be edited.
- Transactions can be deleted by long-pressing in Activity; editing will be added later.
- This is a development prototype, **not ready for App Store release**. Security, backup, accessibility, testing, privacy disclosures and more are needed.
