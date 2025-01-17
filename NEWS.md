<!-- NEWS.md is maintained by https://cynkra.github.io/fledge, do not edit -->

# mockr 0.2.0.9002 (2022-12-30)

- Internal changes only.


# mockr 0.2.0.9001 (2022-12-24)

- Harmonize yaml formatting.

- Revert changes to matrix section.

- Merge pull request #30 from krlmlr/cran-0.2.0.




# mockr 0.2.0.9000 (2022-04-02)

- Same as previous version.


# mockr 0.2.0 (2022-04-02)

## Breaking changes

- `with_mock()` now requires braces (so that error locations can be reported more accurately) and supports only one expression (#15).

## Features

- Functions declared in evaluation environments are now also replaced, with a warning (#5).
- New `local_mock()` (#6).
- `with_mock()` works when running a `testthat::test_that()` block interactively (#7).
- New `get_mock_env()` to make the mocking environment explicit (#7).
- Functions that start with a dot can be mocked (#3, #4).


## Documentation

- Add "Getting started" vignette (#22).

## Internal

- Switch to rlang (#13).
- Switch to GitHub Actions (#10).


# mockr 0.1 (2017-04-28)

Initial CRAN release.

- `with_mock()` modeled closely after `testthat::with_mock()`, can only mock in the package under test but avoids fiddling with R's internals.
    - The `.env` argument now can be a character, but using this argument may lead to different results than `testthat::with_mock()`.
