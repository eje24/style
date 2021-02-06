# style
Temporary container for eje.sty. Many thanks to Jason Chen, from whose style file this one drew significant inspiration (structurally and otherwise).

## To-do:
1. do numbered tcolorbox numbered environments :white_check_mark:
2. do regular numbered environments :white_check_mark:
3. implement current problem + current pset with pset/problem counters
4. reset counters as appropriate when in certain pset mode
5. san serif (formal mode)
6. get rid of extra ifs
7. highlighting and hyperrefs


## Package Options

Below is a list of currently supported options. For additional and option-specific settings, see [additional settings](#additional_settings).

| Option | Default | Functionality |
| --- | --- | --- |
| pset | off | Include this option if you're writing a pset. Additional functionality is described below in [pset settings](#pset_settings).  |
| formal | off | TODO |
| nodate | off | TODO | 
| noheader | off | Include this option if you don't want a header. Additional header functionality is described below in [header settings](#header_settings). |
| marginnum | off | Include this option to put section numbers in the margin. |
| monochrome | Emerald | TODO - A string option. Include  <code> monochrome=COLOR_NAME </code> to switch all tcolorboxes to <code> COLOR_NAME </code>. For a list of color options, see [here](https://en.wikibooks.org/wiki/LaTeX/Colors). |

## <a name="additional_settings"></a> Additional Settings
Additional settings can be specified in the preamble of your document. Some general ones are listed below.

| Setting | Default | How to Change|
| --- |---  |--- |
| Name | Ben Bitdiddle | To set the name to <code>NAME</code>, add <code>\setname{NAME}</code> to the preamble of your document. |
| | | |

###  <a name="pset_settings"></a> pset Settings
There are two pset settings ... BLAH BLAH FILL THIS PART IN.

| Setting | Default | How to Change|
| --- |---  |--- |
| Class | 0.000 |  To set the name to <code>CLASS</code>, add <code>\setpsetclass{CLASS}</code> to the preamble of your document. |
| Style | standalone | To set the style to <code>STYLE</code>, add <code>\setpsetclass{STYLE}</code> to the preamble of your document. |

### <a name="header_settings"></a> Header Settings 
| Setting | Default | How to Change|
| --- |---  |--- |
| | | |

###  <a name="color_settings"></a> Color Settings
| Setting | Default | How to Change|
| --- |---  |--- |
| | | |

## <a name="examples"></a> Examples


## Packages:
This style file uses the following packages.
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
- Placing <code>\setdefcolor{Emerald}</code> (or any other color) immediately before <code>\begin{document}</code> results in an error. Placing it after <code>\begin{document}</code>, or placing another command, such as </code>\setpsetstyle{series}</code> between the two resolves this issue.

If you find another - let me know!

## Far-future:
- add in algorithm support
- add in minted support (for python and similar)