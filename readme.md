- [About us](#about-us)
- [Prerequisites](#prerequisites)
- [Project proposals](#project-proposals)
  * [Overview](#overview)
  * [Where to submit proposals](#where-to-submit-proposals)
  * [Proposal outline](#proposal-outline)
- [Ideas for discussion](#ideas-for-discussion)
  * [Semantic parser](#semantic-parser)
  * [Improving test integration in the elm languague server](#improving-test-integration-in-the-elm-languague-server)
  * [Improve pure Elm markdown parser](#improve-pure-elm-markdown-parser)
  * [Smart generators in the language server](#smart-generators-in-the-language-server)

# About us

We're a organization focusing on the functional progamming language [Elm](elm-lang.org/). We're not working on the comipler, but on things that are related to tooling for the ecosystem and other improvements for users of the language.

So far this organization owns a parser/lexer for Elm, a language server which in a good state and additional packages, that make working with Elm a breeze. Most of these are written in Typescript or Elm.

If we're selected as a mentoring organization for 2021, students will need to review the overview of a good project proposal, follow the outline for proposals when applying, and review the list of project ideas detailed below. Students are welcome to propose ideas outside the list and are encouraged to be as creative as they like.

If you want to work on any of these, please reach out, we don't care about your gender, skin color, religion etc. pp. 
All are welcome <3

# Prerequisites
Some coding skills, basic familiarity with Git, solid understanding and interest in programming. Ability to quickly understand existing code is beneficial. 

# Project proposals

## Overview
Qualifications for a good Summer of Code proposal:

    Discrete, well-defined, modular
    Comprised of a series of measurable sub-goals
    Based on open specs that are available free of charge
    Based on complete specs

An example of a good proposal is the implementation of a new feature or function that is not yet available yet.

An example of a less desirable proposal is one that's not as measurable, such as refactoring something.

To re-iterate:

    Localized/isolated code projects = good
    Global code refactoring = bad
    A project should have a set of subgoals, so even if the end goal turns out to be too big some of the parts will be of benefit.
    Not too big! This is an important problem when choosing a project, while it is fun to think about solving a grand project its not always realistic. Its better to finish a smaller project than to start a grand one.
    
## Where to submit proposals
In addition to submitting to the [Google Summer of Code website](https://summerofcode.withgoogle.com/
), you are highly encouraged to submit your idea/proposal to this repo via issues for discussion. History showed, that students, that reach out early to redefine and focus the scope of their project, are more likely to be selected and successful.

## Proposal outline
Please use this template for your proposal:
```
PROJECT TITLE GOES HERE

    Name:
    Nick in the Elm Slack:
    Summary: A somewhat small but explanatory walk through of the project. It should not be overly detailed just enough to understand the problem trying to be fixed and how this project opt to solve it.
    How will I achieve this: Explain how the project will be done, what technologies are needed and how to implement them.
    What will the project focus on: Explain what the project will focus on, what is the important parts of the project.
    Benefits: Who will benefit and why from this project. Think about what a user or developer may need or do to benefit from it. Why does it benefit many users.
    Timeline: Set some sub goal and try to put dates to these, this is mostly to help you to not over/under estimate, how long it will take you.
    Goals: What is the goal of the project, a project may not always solve the problem entirely as it may take to much time. Think hard about what can be accomplished during a summer with your skill and deduct that quite a bit. If the project can't be done after this perhaps its better to opt for a smaller one or one with subgoals.
    Requirements: What is needed to complete the project, what code language knowledge what hardware etc.
```

# Ideas for discussion

## Semantic parser
Writing a [semantic](https://github.com/github/semantic) parser for Elm will hopefully help getting github to be much smarter about Elm code in the future.

More info can be found here: [Adding new languages](https://github.com/github/semantic/blob/master/docs/adding-new-languages.md)

What's needed: tree sitter, haskell

Possible mentor: TBD

Difficulty: Hard


## Improving test integration in the elm languague server
The [Elm Language Server](https://github.com/elm-tooling/elm-language-server) only has a simple test integration at the moment, consisting of [elm-test](https://github.com/rtfeldman/node-test-runner) being used to parse and validate test files. 

It would be nice to actually be able to run tests from code lenses or a dedicated test panel. Being able to run single tests or groups (might need changes in elm-test) and getting a nice summary of what happened. Coverage integration could be a strech goal.

See these extensions as a reference:
[Java Test Runner by Microsoft](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-test)
[.NET Core Test Explorer](https://marketplace.visualstudio.com/items?itemName=formulahendry.dotnet-test-explorer)

What's needed: typescript, lsp, vscode, elm

Possible mentor: Razzeee

Difficulty: Medium

## Improve pure Elm markdown parser
The current standard markdown parser in Elm, [`elm-explorations/markdown`](http://github.com/elm-explorations/markdown), is a wrapper around marked.js. It is not written in pure Elm, requires a global hljs script to work with syntax highlighting, and [uses an outdated version of marked.js](https://github.com/elm-explorations/markdown/issues/6).

[`dillonkearns/elm-markdown`](https://github.com/dillonkearns/elm-markdown) is a pure Elm markdown parser, and [is built to be extensible](https://elm-pages.com/blog/extensible-markdown-parsing-in-elm). `dillonkearns/elm-markdown` is currently used for a lot of `elm-pages` applications, but there are still some core missing parsing features. It would be great to get that project to the point that it can become the standard markdown parsing library for projects like [the Elm package site](https://github.com/elm/package.elm-lang.org/blob/6e004897f23ffeb71b5d283f1d0042b64ff20a41/src/frontend/Utils/Markdown.elm#L7-L14) and other Elm apps.

There are some parsing areas that are not yet implemented, see [automated markdown spec failures](https://github.com/dillonkearns/elm-markdown/tree/master/test-results/failing/GFM), and the [open issues](https://github.com/dillonkearns/elm-markdown/issues). Goal: get the automated spec tests passing, and clarify places where it needs to diverge from the spec because of its specific handling of HTML for extensibility.

What's needed: elm, parsing, markdown

Possible mentor: Dillon Kearns

Difficulty: ??


## Smart generators in the language server
See this issue for in depth discussions https://github.com/elm-tooling/gsoc-projects/issues/1
