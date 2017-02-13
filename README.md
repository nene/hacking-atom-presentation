# Hacking Atom text editor

## Key bindings

Menu -> Keymap...

Define shortcuts for:

- Close all tabs (avoiding Cmd-W from closing the window)
- Managing files (Delete, Rename, Duplicate)

## Snippets

Menu -> Snippets...

- Jasmine test snippets


## Init script

Menu -> Init script...

`init.js` file.


## Hacking on packages

Using the `apm` tool.

    # First uninstall the original package to not confuse Atom
    # Then install the package from source for development
    $ apm develop <package-name>
    $ cd ~/github/<package-name>
    $ atom -d .

How does `apm init` work?

    # Default is coffeescript
    $ apm init --package <my-package> [--syntax javascript|coffeescript]

    $ apm init -p my-package --syntax javascript

    # Link it for development
    $ cd my-package/
    $ apm link


## Hacking a grammar?

When you look for docs, you'll find lots of confusion as apparently
Atom itself has no docs on working with grammar files.

Atom happens to inherit its grammar definitions from TextMate.
See: http://manual.macromates.com/en/language_grammars

## Some Atom packages I've found useful

- [keyboard-macros](https://atom.io/packages/atom-keyboard-macros) for Atom
- [sublime-style-column-selection](https://atom.io/packages/sublime-style-column-selection) for Atom
- [js-test-toggler](https://github.com/nene/js-test-toggler) for jumping between tests and code in XRebel
- [cucumber-step](https://github.com/nene/atom-cucumber-step) for jumping between .feature files and .js implementation
- [blame](https://atom.io/packages/blame) show Git blame as gutter
- [git-time-machine](https://atom.io/packages/git-time-machine) visual view of Git commit history of a file
- [docblockr](https://atom.io/packages/docblockr) a helper package for writing doc-comments
- [activate-power-mode](https://atom.io/packages/activate-power-mode) the best of them all :)
