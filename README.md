# An Emacs mode for Zeek scripts

This is a very basic Emacs major mode for Zeek scripts. Supported features:

- Syntax highlighting

- Script formatting and parsing via [zeekscript](https://github.com/zeek/zeekscript),
  when available: `C-c C-f` formats the current buffer; `C-c C-p` parses it and renders
  the parse tree into a new buffer.

- Whitespace configuration: `TAB` always inserts tab character. The mode also highlights
  trailing whitespace as well as spaces used after tabs.

Automatic indentation isn't yet supported, but use of `zeekscript` for
formatting approximates it.

## Installation

Place `zeek-mode.el` in a directory accessible to Emacs and source it as follows:

    (require 'zeek-mode)
