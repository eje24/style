# style
Temporary container for eje.sty. Heavily based off of chez.sty.

## To-do:
1. do numbered tcolorbox numbered environments
2. do regular numbered environments
3. implement current problem + current pset with pset/problem counters
3. san serif (formal mode)
4. get rid of extra ifs

## Far-future:
- add in algorithm support
- add in minted support (for python and similar)



## Packages:
This style file uses the following packages
| Package  | Use  |
|---|---|
| xparse  | For greater control over arguments.  |
| xstring |  For extended string functionality |
| etoolbox | For patching commands (such as <code> \patchcmd </code>), and extended boolean functionality.  |
| kvoptions  | For extended option functionality (e.g. passing in string options)  |
| scrlayer-scrpage  | For KOMA-script header functionality. (KOMA doesn't like fancyhdr) |
|  subfiles |   |
| xcolor | For fancy colors. |
| graphicx  | For fancy graphics and image handling  |
| lmodern  |  Font stuff |
| cmbright  | Font stuff |
| lato  |  Font stuff |
|  microtype |  Font stuff |
|  setspace | Line spacing |
|  geometry |   |
| tikz | For TikZ diagrams.|
| enumitem | For lists|
| tcolorbox | For color box environments. |
| hyperref | For hyperlinks. |
| cleveref | Smarter theorem referencing (currently unused) |