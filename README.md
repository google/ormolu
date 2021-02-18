# Ormolu

**This is not an official Google product.**

**This is Google's fork of the original Tweag's
[Ormolu](https://github.com/tweag/ormolu) repository with a few
changes on top of it.**

Notable differences from the original Ormolu:

*   Commas come at the beginning for tuples and lists
*   In type signatures, arrows and double-colons come at the beginning
*   Less vertical space for parenthesized multi-line code

## Maintaining the Repository

We occasionally pull in upstream changes from the Tweag's repository.
Because there are very few deviations from the original Ormolu, we
want to make them prominent by always having them on top of the commit
chain. So when we pull in upstream changes, follow this procedure.

1.  Pull Tweag's `master` branch into the `master` branch of this repo
2.  Rebase the `gfork` branch on top of `master`
3.  Verify all the tests pass; fix them if not

You may encounter merge conflicts at step 2. Please resolve them
properly.

One downside of rebasing is that the hashes of the commits in the
`gfork` branch change every time the rebase happens on top of the new
`master`. This is a small price we have to pay to have the deviating
commits clearly visible.
