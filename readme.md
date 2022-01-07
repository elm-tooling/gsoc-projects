- [About us](#about-us)
- [Prerequisites](#prerequisites)
- [Project proposals](#project-proposals)
  * [Overview](#overview)
  * [Where to submit proposals](#where-to-submit-proposals)
  * [Proposal outline](#proposal-outline)
- [Ideas for discussion](#ideas-for-discussion)
  * [Smart generators in the language server](#smart-generators-in-the-language-server)
  * [Notebook support for VSCode](#notebook-support-for-vscode)

# About us

We're an organization focusing on the functional progamming language [Elm](https://elm-lang.org/). We're not working on the compiler, but on things that are related to tooling for the ecosystem and other improvements for users of the language.

So far this organization owns a parser/lexer for Elm, a language server which is in a good state, and additional packages, that make working with Elm a breeze. Most of these are written in Typescript or Elm, but we do have some Haskell too.

If we're selected as a mentoring organization for 2021, students will need to review the overview of a good project proposal, follow the outline for proposals when applying, and review the list of project ideas detailed below. Students are welcome to propose ideas outside the list and are encouraged to be as creative as they like.

If you want to work on any of these, please reach out. We don't care about your gender, skin color, religion etc. pp. 
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
    Not too big! This is an important problem when choosing a project, while it is fun to think about solving a grand project, it's not always realistic. It's better to finish a smaller project than to start a grand one.
    
## Where to submit proposals
In addition to submitting to the [Google Summer of Code website](https://summerofcode.withgoogle.com/), you are highly encouraged to submit your idea/proposal to this repo via issues for discussion. History has shown that students who reach out early to refine and focus the scope of their project are more likely to be selected and successful.

## Proposal outline
Please use this template for your proposal:
```
PROJECT TITLE GOES HERE

    Name:
    Nick in the Elm Slack:
    Summary: A somewhat small but explanatory walkthrough of the project. It should not be overly detailed, just enough to understand the problem trying to be fixed and how this project opts to solve it.
    How will I achieve this: Explain how the project will be done, what technologies are needed, and how to implement them.
    What will the project focus on: Explain what the project will focus on and what the important parts of the project are.
    Benefits: Who will benefit from this project and why. Think about what a user or developer may need or do to benefit from it. Why does it benefit many users.
    Timeline: Set some subgoals and try to put dates to these, this is mostly to help you to not over/under estimate, how long it will take you.
    Goals: What is the goal of the project. A project may not always solve the problem entirely as it may take too much time. Think hard about what can be accomplished during a summer with your skills and deduct from that quite a bit. If the project can't be done after this, perhaps it's better to opt for a smaller one or one with subgoals.
    Requirements: What is needed to complete the project, what code language knowledge, what hardware, etc.
```

# Ideas for discussion

## Smart generators in the language server
See this issue for in depth discussions https://github.com/elm-tooling/gsoc-projects/issues/1


## Notebook support for VSCode
We would like to support Elm Notebooks, for datascience and similar. One path for this to get easier would be implementing the proposed vscode api here: https://code.visualstudio.com/api/extension-guides/notebook

Possible Mentor: Kolja Lampe (razzeee)

Difficulty: Medium


