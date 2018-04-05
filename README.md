# cointop

> Coin tracking for hackers

[![License](http://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/miguelmota/cointop/master/LICENSE.md) [![Build Status](https://travis-ci.org/miguelmota/cointop.svg?branch=master)](https://travis-ci.org/miguelmota/cointop) [![Go Report Card](https://goreportcard.com/badge/github.com/miguelmota/cointop?)](https://goreportcard.com/report/github.com/miguelmota/cointop) [![GoDoc](https://godoc.org/github.com/miguelmota/cointop?status.svg)](https://godoc.org/github.com/miguelmota/cointop)

<img src="./assets/screenshot-001.gif" width="880" />

[`cointop`](https://github.com/miguelmota/cointop) is a fast and lightweight interactive terminal based UI application for tracking and monitoring cryptocurrency coin stats in real-time. The interface is inspired by [`htop`](https://en.wikipedia.org/wiki/Htop).

## Features

- Quick sort shortcuts
- Vim style keys
- Pagination
- Color coded

#### Future releases

- Advanced search
- "Favorites" list
- Coin charts
- Currency conversion (i.e. Euro, Yen)
- Markets/Exchanges
- CryptoCompare API

## Install

Make sure to have [go](https://golang.org/) (1.9+) installed, then do:

```bash
go get -u github.com/miguelmota/cointop
```

<!--
#### Alternatively (without go)

```
sudo curl -s "https://raw.githubusercontent.com/miguelmota/cointop/master/install.sh?$(date +%s)" | bash
```
-->

## Usage

```bash
$ cointop
```

### Table commands

List of shortcuts:

Key|Action
----|------|
<kbd>↑</kbd>|navigate up
<kbd>↓</kbd>|navigate down
<kbd>→</kbd>|next page
<kbd>←</kbd>|previous page
<kbd>Page Up</kbd>|page up
<kbd>Page Down</kbd>|page down
<kbd>Home</kbd>|navigate to first line of page
<kbd>End</kbd>|navigate to last line of page
<kbd>Enter</kbd>|visit highlighted coin on CoinMarketCap
<kbd>Esc</kbd>|alias to quit
<kbd>Space</kbd>|alias to enter key
<kbd>Ctrl</kbd>+<kbd>c</kbd>|alias to quit
<kbd>Ctrl</kbd>+<kbd>d</kbd>|page down (vim style)
<kbd>Ctrl</kbd>+<kbd>n</kbd>|next page (vim style)
<kbd>Ctrl</kbd>+<kbd>p</kbd>|previous page (vim style)
<kbd>Ctrl</kbd>+<kbd>r</kbd>|force refresh
<kbd>Ctrl</kbd>+<kbd>u</kbd>|page up (vim style)
<kbd>0</kbd>|navigate to first page (vim style)
<kbd>1</kbd>|sort by *[1] hour change*
<kbd>2</kbd>|sort by *[2]4 hour change*
<kbd>7</kbd>|sort by *[7] day change*
<kbd>a</kbd>|sort by *[a]vailable supply*
<kbd>g</kbd>|navigate to first line of page  (vim style)
<kbd>G</kbd>|navigate to last line of page (vim style)
<kbd>h</kbd>|previous page (vim style)
<kbd>H</kbd>|navigate to top of table window (vim style)
<kbd>j</kbd>|navigate down (vim style)
<kbd>k</kbd>|navigate up (vim style)
<kbd>l</kbd>|next page (vim style)
<kbd>L</kbd>|navigate to last line of table window (vim style)
<kbd>m</kbd>|sort by *[m]arket cap*
<kbd>M</kbd>|navigate to middle of table window (vim style)
<kbd>n</kbd>|sort by *[n]ame*
<kbd>p</kbd>|sort by *[p]rice*
<kbd>r</kbd>|sort by *[r]ank*
<kbd>s</kbd>|sort by *[s]ymbol*
<kbd>t</kbd>|sort by *[t]otal supply*
<kbd>u</kbd>|sort by *last [u]pdated*
<kbd>v</kbd>|sort by *24 hour [v]olume*
<kbd>q</kbd>|[q]uit
<kbd>$</kbd>|navigate to last page (vim style)

<!--
|`h`|toggle [h]elp|
|`?`|alias to help|
-->

## FAQ

- Q: Where is the data from?

  - A: The data is from [Coin Market Cap](https://coinmarketcap.com/).

- Q: What coins does this support?

  - A: This supports any coin listed on [Coin Market Cap](https://coinmarketcap.com/).

- Q: How often is the data polled?

  - A: Data gets polled once every minute by default.

- Q: I installed cointop without errors but the command is not found.

  - A: Make sure your `GOPATH` and `PATH` is set correctly.
    ```bash
    export GOPATH=$HOME/go
    export PATH=$PATH:$GOPATH/bin
    ```

- Q: What is the size of the binary?

  - A: The executable is only ~1.9MB in size.

## Authors

- [Miguel Mota](https://github.com/miguelmota)

## License

Released under the MIT license.
