# hledger User Cookbook

<div class=pagetoc>

<!-- toc -->
</div>

**Goal for 2022:** This page aims to become the comprehensive list of concrete, actionable, task-oriented advice for hledger users on how to tackle common real-world problems, using hledger where possible, but pointing to other tools if more effective, and including placeholders where we don't yet have a good answer.

**See also:**
- <https://plaintextaccounting.org> and <https://wiki.plaintextaccounting.org> collect similar but more generic advice for any and all PTA tools.
- If you don't yet know the basics of hledger, see the [home page](index.md), eg [How to get started](index.md#how-to-get-started).
- When you find something that's not covered here, or you have a suggestion, we'd appreciate [a chat message](support.md) (or email).

<!--
Documentor tips:
Big pages while practical, additional subpages when needed. 
Include minimal answers/inline examples when feasible, followed by links to longer answers/related resources. 
Check plaintextaccounting.org's and wiki.plaintextaccounting.org's categories.
-->

<!-- two column layout, interferes with editing in Obsidian, skip for now
<div style="float:left;">
</div>
<div style="float:right;">
</div>
<br clear=all>
-->

The cookbook falls into two parts: 
the [General usage](#general-usage) of hledger,
and [Accounting and bookkeeping](#accounting-and-bookkeeping) examples.

## General usage
<!-- sections ordered roughly by need -->

### Data entry
- [Create a journal](create-a-journal.md)
- [Importing CSV data](import-csv.md)

### Preserving your data
- [Track changes with version control](track-changes-with-version-control.md)
- Keep backups - [3-2-1 rule](https://en.wikipedia.org/wiki/Backup#3-2-1_rule)

### Checking for errors
- [Checking for errors](checking-for-errors.md)
- [Balancing the accounting equation](balancing-the-accounting-equation.md)

### Reporting techniques
- [Report examples](report-examples.md)
- [Tags tutorial](tags-tutorial.md)
- [Rewrite account names](rewrite-account-names.md)
- [Rewrite commodity symbols](rewrite-commodity-symbols.md)

### Making charts
- [Charts and Graphs](charts.md)

### Customising
- [Change account name separator](change-account-name-separator.md)
- [Command line completion](command-line-completion.md)
- [Editor configuration](editors.md)
- [Save frequently used options](save-frequently-used-options.md)
- [Scripting hledger](scripting.md)

### Setups and workflows
- [Getting Started](start.md)
- [Common workflows](common-workflows.md)

### Other user interfaces
- [hledger-web tips](hledger-web-tips.md)
- [Mobile apps](mobile-apps.md)

### Other software
- [Exporting from hledger](export.md)
- [hledger and Beancount](beancount.md)
- [hledger and dsq / DataStation](dsq.md)
- [hledger and GnuCash](gnucash.md)
- [hledger and Ledger](ledger.md)
- [hledger and Obsidian](obsidian.md)
- [hledger and Postgres](postgres.md)
- [hledger and Quicken/Quickbooks](quicken.md)
- [hledger and SQLite](sqlite.md)
- [hledger and Ultorg](ultorg.md)
- [hledger and YNAB](ynab.md)

## Accounting and bookkeeping
<!-- sections ordered mostly alphabetically -->

### Learning accounting and bookkeeping
- [Accounting concepts](accounting.md)
- [Common journal entries](common-journal-entries.md)
- [pta.o: Choosing cash or accrual](https://plaintextaccounting.org/#choosing-cash-vs-accrual)

### Borrowing and lending
- [Borrowing and lending](loans.md)

### Budgeting
- [Budgeting](budgeting.md)
<!-- ### Depreciation -->
<!-- [Depreciation](http://rantsideasstuff.com/posts/2018/07/08-depreciation-in-personal-finance-with-hledger) -->

### Eco accounting
- [PTA wiki: Eco accounting](https://wiki.plaintextaccounting.org/Eco-accounting)

### Forecasting
- [Forecasting](forecasting.md)

### Inventory tracking
- [Tracking and selling inventory](inventory.md)
- [PTA wiki: Inventory](https://github.com/plaintextaccounting/plaintextaccounting/wiki/Inventory)

### Investing and trading
- [Track investments (2017)](track-investments.md)
- [Track investments (2020)](investments.md)
- [Calculate unrealized gain](gain.md)
- [Calculate return on investment](roi.md)
- [hledger-fifo](scripts.md#hledger-fifo)

### Invoicing
- [Invoicing](invoicing.md)
- [Project accounting](project-accounting.md)

### Multiple currencies
- [Currency conversion](currency-conversion.md) and 
  [Currency conversion 2](conversion2.md)
- [Multicurrency tutorial (2018)](multicurrency-tutorial.md)

### Non-profit accounting

### Taxes

### Time tracking
- [Converting time to money](time-to-money.md)
- [Time planning](time-planning.md)

### Trip expenses
- [Foreign trip expenses](foreign-trip-expenses.md)

### Shared expenses

