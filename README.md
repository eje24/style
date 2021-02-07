# style
<p>Temporary container for eje.sty. Many thanks to Jason Chen, from whose style file this one drew significant inspiration (structurally and otherwise). </p>

## To-do:
* implement \newpset{name or number} and \newpsetproblem{name or number}
    - redefine section so it says "Problem X" instead of "1.1 Problem 1"
* implement current problem + current pset with pset/problem counters
* proof and solution environments
* reset counters as appropriate when in certain pset mode
* san serif (formal mode)
* get rid of extra ifs
* highlighting and hyperrefs
* error handling + checking that KOMA is properly loaded 
* footnotes



## Table of Contents
1. [Package Options](#package_options)
2. [Environments](#environments)
3. [Additional Settings](#additional_settings)
4. [Quick-Setup for psetting](#psetting)
5. [Examples](#examples)
6. [Packages](#packages)
7. [Known Bugs](#known_bugs)
8. [Future Features](#future_features)


## <a name="package_options"></a> Package Options

Below is a list of currently supported options. For additional and option-specific settings, see [additional settings](#additional_settings).

| Option | Default | Functionality |
| --- | --- | --- |
| pset | off | Include this option if you're writing a pset. Additional functionality is described below in [pset settings](#pset_settings).  |
| formal | off | TODO |
| nodate | off | TODO | 
| noheader | off | Include this option if you don't want a header. Additional header functionality is described below in [header settings](#header_settings). |
| marginnum | off | Include this option to put section numbers in the margin. |
| monochrome | Emerald | TODO - A string option. Include  <code> monochrome=COLOR_NAME </code> to switch all tcolorboxes to <code> COLOR_NAME </code>. For a list of color options, see [here](https://en.wikibooks.org/wiki/LaTeX/Colors). |

## <a name="environments"></a> Environments

## <a name="additional_settings"></a> Additional Settings
Additional settings can be specified in the preamble of your document. Some general ones are listed below.

| Setting | Default | What|
| --- |---  |--- |
| Name | Ben Bitdiddle | Your name. To set the name to <code>NAME</code>, add <code>\setname{NAME}</code> to the preamble of your document. |
| | | |


### <a name="header_settings"></a> Header Settings 
| Setting | Default | What  |
| --- |---  |--- |
| | | |

###  <a name="color_settings"></a> Color Settings
For coloring purposes, boxed theorem environments are partitioned into three groups: **plain**, **def(inition)**, and **remark**. The groups are as follows.

* plain: <code>theorembox</code>, <code>lemmabox</code>, <code>propbox</code> (proposition)
* def: <code>corollarybox</code>, <code>conjecturebox</code>, <code>claimbox</code>, <code>defbox</code> (definition)
* remark: <code>remarkbox</code>

These correspond to the three theoremstyles provided by the <code> amsthm </code> package. Colors can be set for each of these groups separately, as described below.
| Setting | Default | What |
| --- |---  |--- |
| plaincolor | Periwinkle | The color of the plain group. Can be set to <code> COLOR </code> by adding <code> \setplaincolor{COLOR}</code> to the preamble. |
| defcolor | Emerald | The color of the def group. Can be set to <code> COLOR </code> by adding <code> \setdefcolor{COLOR}</code> to the preamble.  |
| remarkcolor | CornflowerBlue | The color of the remark group. Can be set to <code> COLOR </code> by adding <code> \setremarkcolor{COLOR}</code> to the preamble.  |
| linkcolor | | TODO - hyperref stuff |


###  <a name="pset_settings"></a> pset Settings
If you're typing up a single pset assignment... BLAH BLAH FILL THIS IN

| Setting | Default | What |
| --- |---  |--- |
| Class | 0.000 |  The class to which this homework/pset belongs. To set the name to <code>CLASS</code>, add <code>\setpsetclass{CLASS}</code> to the preamble of your document. |
| Style | standalone | To set the style to <code>STYLE</code>, add <code>\setpsetstyle{STYLE}</code> to the preamble of your document. |


## <a name="examples"></a> Examples

### <a name="pset_example"></a> pset Example

### <a name="formal_example"></a> formal example

### <a name="misc_example"></a> Miscellaneous Example


## <a name="packages"></a> Packages:
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

## <a name="known_bugs"></a>Known Bugs:
- Placing <code>\setdefcolor{Emerald}</code> (or any other color) immediately before <code>\begin{document}</code> results in an error. Placing it after <code>\begin{document}</code>, or placing another command, such as <code>\setpsetstyle{series}</code> between the two resolves this issue.

If you find another, please let me know!

## <a name="future_features"></a> Future features:
- add in algorithm support
- add in minted support (for python and similar)