# Shell script for tradelog analisys
### Usage:
   - ./tradelog [-h|--help]
   - ./tradelog [FILTER...] [COMMAND] [LOG [LOG2 [...]]]
### Commands, one from:
<pre>
   list-tick         Print all tickers
   profit            Print profit
   pos               Print list of values of held positions for each ticker
   last-price        Print last known price for each ticker
   hist-ord          Print histogram of the number of transactions for each ticker
   graph-pos         Print graph of values of held positions for each ticker
</pre>
### Filters, can be a combination of:
<pre>
   -a DATETIME       Process only dates after  (Format: YY-MM-DD HH-MM-SS)
   -b DATETIME       Process only dates before (Format: YY-MM-DD HH-MM-SS)
   -t TICKER         Process only selected tickers
   -w WIDTH          Maximum width of line (Commands: hist-ord OR graph-pos)
                     More than one occurrence of an WIDTH argument will produce an error
</pre>
### The script can process records compressed with the gzip tool.
