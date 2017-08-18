# t #

## Description ##

t is a shell script for working with [ledger][]'s [timelog][] format.

## Install ##

Download and install the script to a `bin` directory that exists in your `$PATH`. For example, `$HOME/bin`:

    curl --silent -G https://raw.github.com/nuex/t/master/t -o ~/bin/t
    chmod +x ~/bin/t

Set the location of your timelog file:

    export $TIMELOG=$HOME/.timelog.ldg

The default location is `$HOME/.timelog.ldg`.

If you clone the entire repository instead then you'll also get a zsh
completion function.

## Usage ##

Usage: `t <action>`

### Actions ###

- `t in` - clock into project or last project
- `t out` - clock out of project
- `t sw,switch` - switch projects
- `t bal` - show balance
- `t hours,today` - show balance for today
- `t week` - show balance beginning most recent Monday
- `t month` - show balance beginning 1st of current month
- `t edit` - edit timelog file
- `t cur` - show currently open project
- `t last` - show last closed project
- `t grep` - grep timelog for argument
- `t cat` - show timelog
- `t less` - show timelog in pager
- `t timelog` - show timelog file

## References ##

Even though this works with [ledger][] 3, the [timelog][] format is only referenced in the [ledger][] v2 documents.  Here are a few resources about the [timelog][] format:

- [Using timeclock to record billable time][timelog]
- [timelog files][htl] - from the [hledger][] project

[ledger]: http://ledger-cli.org
[timelog]: http://ledger-cli.org/2.6/ledger.html#Using-timeclock-to-record-billable-time
[htl]: http://hledger.org/MANUAL.html#timelog-files
[hledger]: http://hledger.org/
