# Common workflows

<div class=pagetoc>

<!-- toc -->
</div>

There are lots of ways to use hledger; here is an overview.
Of course you can mix and match these.

In all of these workflows, remember to back up your files
periodically to safeguard your financial data.

## Web UI

Probably the easiest hledger workflow, if it works:

Download and run `hledger-web`, eg by double-clicking on it.
It should open in your web browser.
Use the add form to add transactions.
It will store data in its default location.
(So you'll see your transactions next time you run it.)

[Tutorial: hledger-web](web.html) describes this in more detail.

## Command line

At a terminal prompt, run `hledger add` and follow the interactive prompts to enter transactions.
It will store data in its default location.
Run `hledger` to list commands to try.
Eg, run
`hledger bs` to see your account balances (a [balance sheet]), and
`hledger is` to see your income and expenses (an [income statement]).

[Tutorial: hledger add](add.md) describes this process, and hledger's basic concepts and file format, step by step.
You might want to skim through this one even if you don't plan to use `hledger add`.

## Text editor

Open your preferred text editor and create a journal file, `.hledger.journal` in your home directory.
(Or elsewhere, and set its path in the `LEDGER_FILE` environment variable.)
Create transactions by hand using [journal file](hledger.html) format.
Once you have a few, you can copy/paste them to make more.
When you want more assistance, set up an [editor mode](editors.html).
Here's an example:

```journal
; $HOME/.hledger.journal

2020-01-01 opening balances
    assets:checking         $1234
    equity

2020-03-15 client payment
    assets:checking         $2000
    income:consulting

2020-03-20 Sprouts
    expenses:food:groceries  $100
    assets:cash               $40
    assets:checking
```

Run `hledger` in a terminal to see reports, as in the Command line workflow. Eg:

```shell
$ hledger bs
Balance Sheet 2020-03-20

             || 2020-03-20 
=============++============
 Assets      ||            
-------------++------------
 assets      ||      $3134 
   cash      ||        $40 
   checking  ||      $3094 
-------------++------------
             ||      $3134 
=============++============
 Liabilities ||            
-------------++------------
-------------++------------
             ||            
=============++============
 Net:        ||      $3134 

$ hledger is -M
Income Statement 2020-01-01-2020-03-20

                         || Jan  Feb    Mar 
=========================++=================
 Revenues                ||                 
-------------------------++-----------------
 income:consulting       ||   0    0  $2000 
-------------------------++-----------------
                         ||   0    0  $2000 
=========================++=================
 Expenses                ||                 
-------------------------++-----------------
 expenses:food:groceries ||   0    0   $100 
-------------------------++-----------------
                         ||   0    0   $100 
=========================++=================
 Net:                    ||   0    0  $1900 
```

## Text UI

Use `hledger add` once (see above) to create a journal file.
Now run `hledger-ui` to view account balances.
Use the onscreen help to get around.
Eg, press `a` to add a transaction, and follow the prompts (it uses `hledger add`).

[Tutorial: hledger-ui](ui.md) describes this setup in more detail.

## CSV import

Download CSV files from banks and financial institutions, manually or
using tools/services that automate this (ledger_autosync, Plaid, plaid2qif, Tiller etc.)
Use hledger's import command to convert and import the new transactions,
and use any of the hledger UIs to see reports.

[Importing CSV data](import-csv.md) is a quick tutorial on the importing from CSV part.
Some downloading helpers can be found at
<https://plaintextaccounting.org/#data-importconversion> (search for "download").


## Some more advanced workflows

- Notes on [Simon's setup](simons-setup.html)

- Dmitry Astapov's Full-fledged Hledger workflow (tutorial):\
  <https://github.com/adept/full-fledged-hledger>

- Andreas Pauley's hledger-flow workflow (tutorial & slideshow):\
  <https://github.com/apauley/hledger-flow>

- rotorkunstkultur's setup for chaotic German freelancers:\
  <https://github.com/rotorkunstkultur/rtrledger>

- Michael Walker's personal finance setup:\
  <https://memo.barrucadu.co.uk/personal-finance.html>


[convert]:           convert-csv-files.html
[import]:            hledger.html#import
[balance sheet]:     https://en.wikipedia.org/wiki/Balance_sheet#Personal
[income statement]:  https://en.wikipedia.org/wiki/Income_statement

