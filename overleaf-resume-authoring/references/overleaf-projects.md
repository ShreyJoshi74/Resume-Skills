# Overleaf resume project reference

Use this reference when changing a project structure, compiler, fonts, links, or compiling/debugging source.

## Project invariant

Overleaf compiles one editable plain-text Main document. Keep the main `.tex` file in the project root; set it explicitly in **Settings → Compiler → Main document** when a project has multiple `.tex` files. Source: [Overleaf: The Main document](https://docs.overleaf.com/getting-started/recompiling-your-project/the-main-document).

## Compiler routing

- Retain the current compiler unless its requirements conflict with the requested content or assets.
- pdfLaTeX is Overleaf's default and supports common PNG, JPG, and PDF assets.
- XeLaTeX and LuaLaTeX are appropriate for OpenType/TrueType fonts, robust Unicode, and non-Latin scripts. `fontspec` requires XeLaTeX or LuaLaTeX; remove obsolete `inputenc`/`fontenc` setup when migrating to those engines.
- Recompile twice when cross-references or a bibliography need resolution. 

Sources: [Choosing a LaTeX Compiler](https://www.overleaf.com/learn/latex/Choosing_a_LaTeX_Compiler), [XeLaTeX](https://www.overleaf.com/learn/latex/XeLaTeX), [Multilingual typesetting with polyglossia and fontspec](https://www.overleaf.com/learn/latex/Multilingual_typesetting_on_Overleaf_using_polyglossia_and_fontspec).

## Links and failures

`hyperref` supplies `\href` and `\url`; it is normally loaded late in the preamble. A missing package is a common cause of undefined environments or commands. For an Overleaf-only project, use **Recompile**, inspect the first meaningful log error, repair the source or package dependency, then recompile.

Sources: [Hyperlinks](https://www.overleaf.com/learn/latex/Hyperlinks), [Environment undefined](https://www.overleaf.com/learn/latex/Errors/LaTeX_Error%3A_Environment_XXX_undefined).
