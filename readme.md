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

## Improve pure Elm markdown parser
The current standard markdown parser in Elm, [`elm-explorations/markdown`](http://github.com/elm-explorations/markdown), is a wrapper around marked.js. It is not written in pure Elm, requires a global hljs script to work with syntax highlighting, and [uses an outdated version of marked.js](https://github.com/elm-explorations/markdown/issues/6).

[`dillonkearns/elm-markdown`](https://github.com/dillonkearns/elm-markdown) is a pure Elm markdown parser, and [is built to be extensible](https://elm-pages.com/blog/extensible-markdown-parsing-in-elm). `dillonkearns/elm-markdown` is currently used for a lot of `elm-pages` applications, but there are still some core missing parsing features. It would be great to get that project to the point that it can become the standard markdown parsing library for projects like [the Elm package site](https://github.com/elm/package.elm-lang.org/blob/6e004897f23ffeb71b5d283f1d0042b64ff20a41/src/frontend/Utils/Markdown.elm#L7-L14) and other Elm apps.

There are some parsing areas that are not yet implemented, see [automated markdown spec failures](https://github.com/dillonkearns/elm-markdown/tree/master/test-results/failing/GFM), and the [open issues](https://github.com/dillonkearns/elm-markdown/issues). Goal: get the automated spec tests passing, and clarify places where it needs to diverge from the spec because of its specific handling of HTML for extensibility.

What's needed: elm, parsing, markdown

Possible mentor: Dillon Kearns
