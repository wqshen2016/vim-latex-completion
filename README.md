# vim-latex-completion
Dictionary and snippet files for editting LaTeX documents on Vim.

The dictionary file works with the standard Vim completion feature. The snippet file is intended to be used with [Neosnippet](https://github.com/Shougo/neosnippet.vim). 

* tex.dict - The dictionary, containing command names.
* tex.snip - The snippet file, containing snippets for environments. Each snippet can be called upon by the environment name itself.

These files include commands and environments from LaTeX2e and amsmath, amscd, amsthm, TikZ packages. More specifically:

* tex.dict virtually contains all command names starting with a backslash (`\`). Exceptions are those with no or only one Latin alphabet just after the backslash (`\#` and `\c` for example) and `\begin`.
* tex.snip contains all environment names, and additionally, `\begin`.
 * Compared to the TeX snippet file bundled with Neosnippet, our tex.snip has the advantage that it is clear which environment is contained and which is not.

We have an intention to expand them so that they cope with other often-used packages under the following principles:
* Do it comprehensively, based on some established document if possible.
* Don't surprise users. Aim somewhere between "perfect" and "just one step away," without implementing any unexpected actions, so that it feels like the air around us.

Note: The `abbr` field of the snippets is written in Japanese for now. This is temporary.
