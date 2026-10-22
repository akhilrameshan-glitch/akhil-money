# Akhil Money

A personal finance tracker designed for local use on your device. The app uses browser localStorage; it does not send your financial records to a server.

## Features

- Dashboard grouped by currency with separate Cash, Bank Accounts, and Credit Card summaries.
- Net position shown independently for each currency (for example, AED and INR); no automatic currency conversion.
- Record expenses, income, same-currency transfers, cross-currency transfers with manually entered sent/received amounts and saved effective exchange rate, and credit-card payments.
- Search/filter transaction activity and export transactions to CSV.
- Monthly income/expense reports, separate Assets and Owes Me reports, and account/net-position reports.
- Budgets, recurring transaction templates, bill reminders, and a local rule-based money helper.
- Multiple cash/bank/credit-card accounts with account currency selection.
- Owes Me ledger: choose the source cash/bank account when lending; repayment selects a receiving account. Lending and repayments update balances and do not count as ordinary expense/income.
- House construction projects: one house record with multiple installments, category, budget, payment history, and accumulated construction cost. Each installment can deduct a manually entered amount from any cash/bank account currency while adding a separately entered cost in the house project currency (for example, deduct AED from a UAE bank and add INR to an Indian house project).
- Other asset purchases (such as vehicles): select the source cash/bank account, deduct the purchase amount, and track the asset separately from ordinary expenses.
- Editable income and expense categories.
- JSON backup and restore.
- Offline-capable service worker for the GitHub Pages site.

## Publish on GitHub Pages

Upload `index.html`, `manifest.json`, `sw.js`, and `icon.svg` to the repository's `main` branch. Keep `README.md`. After GitHub Pages publishes, reopen the website. If an installed iPhone app shows an older cached screen, close and reopen it or refresh the website to let the service worker update.

## Important data note

Records are stored locally in the browser on each device. GitHub Pages publishes the app code, not your financial records. Use Settings → Backup and restore regularly. A backup from one device must be restored manually on another device.
