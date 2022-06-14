# Change Log

## [Unreleased]

## [1.7.0] - 2022-06-14

### Added

- Typescript support for `.ts` and `.tsx` files!
- Readme update to highlight the keys in each shortcut

## [1.6.0] - 2020-02-08

### Added

- React hook snippets for `useState`, `useEffect` imports and statements, and a bootstrap with `useState`. It took me a while to figure out the `useState` statement, because I really wanted the `[state, useState]` destructed variables to use one placeholder and capitalize the first character after `use`. Turns out you can do this with a regexp capture but with the Vim vscode extension it does not play nicely. So it works without Vim, but I haven't figured it out for Vim yet.
- Added a PropTypes (`pt`) snippet for setting up the `MyComponent.propTypes` object in case you decided to add it after creating a component. It uses the filename as the default.
- Here are the new snippet commands (you can see the whole list in the README)
  - [`imrus`](./README.md#imrus--import-react-usestate)
  - [`imrue`](./README.md#imrue--import-react-useeffect)
  - [`imruse` or `imrues`](./README.md#imruse-or-imrues--import-react-usestate-and-useeffect)
  - [`rus`](./README.md#rus--react-usestate-statement)
  - [`rue`](./README.md#rue--react-useeffect-statement)
  - [`rfeus` or `rfes`](./README.md#rfeus-or-rfes--react-component-with-export-after-and-usestate-setup)
  - [`pt`](./README.md#pt--proptypes-object)

### Fixed

- Some snippets, such as `rfpe` (create React component with PropTypes object) would not autocomplete snippets until the entire snippet was exited. This is how VSCode snippets work, however, I have learned that you can set the ending point of a snippet (`$0` for the curious) where you like, rather than the end of the code that was added. This allows the `propTypes` object snippet to behave as intended, without having to hit Escape or Ctrl+Space to type further snippets inside the object.

## [1.5.0] - 2020-02-05

### Added

- Testing: expect.toBe(), expect.toBeNull()
- PropTypes.shape({}) snippets

### Changed

- react-testing-library has updated to @testing-library/react since this project started, and there have been a few changes to best practices and syntax.
  One of those changes is that `.firstChild` is not required when using container to snapshot or query against. `container.firstChild` snippets have switched to simply `container`.
- The `rtlbs` snippet (React Testing Library Bootstrap) has had some updates after watching Kent Dodds updated testing course. `render` is a named export, rather than the default,
  and I've swapped the `setup-tests` file import with the actual package. This is an extra step for me to type, but it's more universally useful. At least that's the hope.

## [1.4.0] - 2019-07-25

### Added

- React Testing Library bootstrap for setting up basic component test with the root name of the file (no file extensions)
- React Testing Library snapshot snippet
- Jest `test` block snippet

## [1.3.0] - 2019-06-11

### Added

- Add Storybook snippet for setting up a basic component story based on the root name of the file (no file extensions)

## [1.2.0] - 2019-06-04

### Added

- Add react component with proptypes and default export snippet

## [1.1.0] - 2019-06-04

### Added

- Add react component snippet without any imports or exports for multi-component files
- Add alternative snippet shortcut `rfe` (react functional export) for `rse` (react stateless functional export) due to hooks allowing state in functional components now

## [1.0.4] - 2019-06-04

### Changed

- Update styled component callback snippets to have a semicolon at the end (required to compile).
- Add reference in readme

## [1.0.0] - 2019-01-19

### Added

- `styled-components-snippets.json` so that styled component css is not flooded with our JS snippets

### Changed

- Moved styled components snippets from `snippets.json` to the new snippet file for styled components
- Changed styled component functions to include their parameter in the default typing area

## [0.4.0] - 2019-01-19

### Added

- Styled Component imports for `styled-components` and `@emotion/styled`
- Styled Component creation snippet
- Styled Component function interpolations

### Changed

- Changed enzyme shortcut from `ime` to `imez` because I use it less and wanted `imes` for `@emotion/styled`

## [0.3.0] - 2018-09-12

### Added

- Testing blocks (e.g. describe, it)
- expect to match snapshot, and expect to equal
- Enzyme shallow and mount imports
- Import React, React with Component, and PropTypes

## [0.2.0] - 2018-08-23

### Added

- Console log group snippets
- React lifecycle method snippets
- PropType snippets

### Changed

- Swapped hard spaces for tab character in multiline snippets with indentation. The `\t` should be more friendly for users with 2 or 4 space tabs (or even 3, if you are Satan incarnate).

## [0.1.0] - 2018-08-19

### Added

- Console log snippets (default and with a color)
