# Google summer of code project ideas

## Semantic parser
Writing a [semantic](https://github.com/github/semantic) parser for Elm will hopefully help getting github to be much smarter about Elm code in the future.

More info can be found here: [Adding new languages](https://github.com/github/semantic/blob/master/docs/adding-new-languages.md)

What's needed: tree sitter, haskell

Possible mentor: TBD


## Improving test integration in the elm languague server
The [Elm Language Server](https://github.com/elm-tooling/elm-language-server) only has a simple test integration at the moment, consisting of [elm-test](https://github.com/rtfeldman/node-test-runner) being used to parse and validate test files. It would be nice to actually be able to run tests from code lenses or a dedicated test panel. Being able to run single tests or groups (might need changes in elm-test) and getting a nice summary of what happened. Coverage integration could be a strech goal.

What's needed: typescript, lsp, vscode, elm

Possible mentor: TBD
