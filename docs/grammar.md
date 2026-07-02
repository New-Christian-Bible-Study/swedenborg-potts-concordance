# Concordance Grammar Definition

## Introduction

This page defines the grammar used for the [Swedenborg Concordance published by the Reverend John Potts in 1900](https://www.newchurchhistory.org/funfacts/indexf5a4.html?p=358). By grammar is meant to the semantics and syntax of the concordance:

- semantics refers the meaning of the various elements of the concordance.
- syntax refers to the rules used for the structure of the concordance and the expected grouping of words and symbols that make up the concordance.

Establishing this grammar then provides a common language to use between editors of the digital version of the concordance and software developers working with code that works with the concordance.

## Structure

At the highest level the concordance consists of entries, with each article containing one or more _principal phrases_, and zero or more _contexts_ providing examples of how these phrases are used.

### Principal phrases

_Note: The bulk of the phrases in the concordance are single words, but to keep the terms being used general, `phrase` will still be used exclusively below._

In general an article will group multiple phrases together when they have a similar meaning. In addition, every phrase includes both the English spelling and Latin spelling.

The example below puts these ideas together:

**Blind, To make**. _Occaecare_.</br>
**Blindness**. _Occaecatio_.

<!-- TODO: Handle footnotes like the one for TRUTH-Verum, Veritas. -->

#### Alphabetical order of principal phrases in an article

The English principal phrases may not always be variations on the same core word. For example,

**Perform, Surpass, Be better.** *Prae stare*.</br>
**Excellent.** *Praestaus*.</br>
**Excellence.** *Praestantia*.

In this case we're [including a comment](editing.md#including-comments)

```
# English word out of alphabetical order
```

right before the word.

#### Related entries

A line following a PP with `See`, `See also`, or `See under` specifies entries where to find further information. In addition, a final line in the list of PPs may be `See...` line.

### Quotes

Each quote begins with a reference to a portion of a work by Swedenborg followed by the context from the quote. This portion can either be to a numbered section of the work, or a numbered subsection. Examples of the syntax used is shown below.

| Reference type |Example |
|--|--|
| Reference to a section | @AC 1120 |
| Reference to a section in the previous work | @5386 |
| Reference to a section/subsection of a work | @AC 10492[2] |
| Reference to a subsection in previous section | @--[5] |
| Reference to a different part of the previous subsection | @--. |
| Reference to the very end of the previous section | @--[e] |
| Reference that spans several sections | @SE 4930-4932 |

<!-- TODO: References to Bible verses -->
<!-- TODO: References to other entries -->

