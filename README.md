# vim-latex-completion
Dictionary and snippet files for editting LaTeX documents on Vim.

The dictionary file works with the standard Vim completion feature; the snippet file is intended to be used with NeoSnippet. 

* `tex.dict` - The dictionary, containing command names.
* `tex.snip` - The snippet file, containing snippets for environments. Each snippet can be called upon by the environment name itself.

These files include commands and environments from LaTeX2e and amsmath, amscd, amsthm packages. More specifically:

* `tex.dict` virtually contains all command names starting with a backslash (`\`). Exceptions are those with no or only one Latin alphabet just after the backslash (`\#` and `\c` for example) and `\begin`.
* `tex.snip` contains all environment names and `\begin`.
 * Compared to the TeX snippet file bundled with NeoSnippet, our `tex.snip` has the advantage that it is clear which environment is contained and which is not.

We have an intention to expand them so that they cope with other often-used packages like amsfonts, amssymb, tikz, and beamer under the following principles:
* Do it comprehensively.
* Don't surprise users. Aim somewhere between "perfect" and "just one step away," without implementing any unexpected actions, so that it feels like the air around us.

Note: The `abbr` fields of the snippets are written in Japanese for now. This is temporary.
