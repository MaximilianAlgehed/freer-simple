# 1.2.1.1 (October 4th, 2019)

- Loosened bounds on `template-haskell` ([#29](https://github.com/lexi-lambda/freer-simple/issues/29)).
- Made some minor internal changes to better support GHC 8.8.

# 1.2.1.0 (November 15th, 2018)

- Improved `makeEffect` from `Control.Monad.Freer.TH` to support more datatypes ([#17](https://github.com/lexi-lambda/freer-simple/pull/17)).

# 1.2.0.0 (October 23rd, 2018)

- Added `Control.Monad.Freer.TH`, which provides a `makeEffect` function that automatically generates boilerplate operations using `send` for an effect ([#15](https://github.com/lexi-lambda/freer-simple/pull/15)).

# 1.1.0.0 (February 20th, 2018)

- Changed the implementation of `LastMember` to avoid an issue similar to the one with `Member` fixed in 1.0.1.1 that could cause the constraint to unnecessarily fail to solve ([#6](https://github.com/lexi-lambda/freer-simple/issues/6)).
- Changed the order of the type variables in `interpretM` to be more consistent with other functions (only relevant in combination with `TypeApplications`).
- Re-exported `(~>)` from `Control.Natural` through `Control.Monad.Freer`.

# 1.0.1.1 (January 31st, 2018)

- Fixed a bug that could cause `Member` constraints to erroneously fail to solve ([#3](https://github.com/lexi-lambda/freer-simple/pull/3)).

# 1.0.1.0 (January 27th, 2018)

- Added `subsume` to `Control.Monad.Freer` for deduplicating effects.
- Added `gets` to `Control.Monad.Freer.State` ([#1](https://github.com/lexi-lambda/freer-simple/pull/1)).

# 1.0.0.0 (December 7th, 2017)

- Initial release.
