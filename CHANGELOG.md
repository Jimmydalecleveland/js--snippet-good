# Change Log

## [Unreleased]

## [0.1.0] - 2018-08-19

### Added

- Console log snippets (default and with a color)

## [0.2.0] - 2018-08-23

### Added

- Console log group snippets
- React lifecycle method snippets
- PropType snippets

### Changed

- Swapped hard spaces for tab character in multiline snippets with indentation. The `\t` should be more friendly for users with 2 or 4 space tabs (or even 3, if you are Satan incarnate).

## [0.3.0] - 2018-09-12

### Added

- Testing blocks (e.g. describe, it)
- expect to match snapshot, and expect to equal
- Enzyme shallow and mount imports
- Import React, React with Component, and PropTypes

## [0.4.0] - 2019-01-19

### Added

- Styled Component imports for `styled-components` and `@emotion/styled`
- Styled Component creation snippet
- Styled Component function interpolations

### Changed

- Changed enzyme shortcut from `ime` to `imez` because I use it less and wanted `imes` for `@emotion/styled`

## [1.0.0] - 2019-01-19

### Added

- `styled-components-snippets.json` so that styled component css is not flooded with our JS snippets

### Changed

- Moved styled components snippets from `snippets.json` to the new snippet file for styled components
- Changed styled component functions to include their parameter in the default typing area

## [1.0.4] - 2019-06-04

### Changed

- Update styled component callback snippets to have a semicolon at the end (required to compile).
- Add reference in readme
