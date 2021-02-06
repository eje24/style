# style
Temporary container for eje.sty. Heavily based off of chez.sty.

## To-do:
1. do numbered tcolorbox numbered environments :white_check_mark:
2. do regular numbered environments :white_check_mark:
3. implement current problem + current pset with pset/problem counters
4. reset counters as appropriate when in certain pset mode
5. san serif (formal mode)
6. get rid of extra ifs


## Package Options

## Additional Functionality



## Packages:
This style file uses the following packages
| Package  | Use  |
|---|---|
| xparse  | For greater control over arguments.  |
| xstring |  For extended string functionality |
| etoolbox | For patching commands (such as <code> \patchcmd </code>), and extended boolean functionality.  |
| kvoptions  | For extended option functionality (e.g. passing in string options)  |
| thmtools  | better theorem declaration syntax |
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

## Known Bugs:
- Placing <code>\setdefcolor{Emerald}</code> immediately before <code>\begin{document}</code> results in an error. Placing it after <code>\begin{document}</code>, or placing another command, such as </code>\setpsetstyle{series}</code> between the two resolves this issue.


## Far-future:
- add in algorithm support
- add in minted support (for python and similar)