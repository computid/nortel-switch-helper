# Nortel Switch Helper

A chap called Steven Mirabito apparently aquired a few Nortel BES1020-48T-PWR gigabit 
managed PoE switches but was dismayed to find that Nortel chose to use a Java applet (?!?)
to handle navigating the built-in web configuration UI. His extension aimed to modernize
the UI and remove the Java dependency. 

I acquired a number of 10/100 Nortel BES110-24T's and found a similar issue. I modified
his code to support this switch.

## Installation
To use it, simply navigate to the switch's web UI (192.168.1.132 if not configured
otherwise) and click the extension's icon in the toolbar.

## Development
Clone this repo, then use Bower to pull down a few dependencies:

```
git clone https://github.com/computid/nortel-switch-helper
cd nortel-switch-helper
bower install
```

To load it into Chrome unpacked, go to the [Chrome extensions page](chrome://extensions/),
check "Developer mode" at the top, then choose "Load unpacked extension." To
pack it yourself, choose "Pack extension" on the same page.
