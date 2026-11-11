# Turing Machine Regex Simulator

A single-file, browser-only teaching tool: type a regular expression, watch it compile to a minimal DFA framed as a read-only Turing machine, and step a test string through it in 3D, 2D or as a transition table.

**Live:** https://jonatcompsage.github.io/RegexTuringTest/

- Everything is in `index.html`; there is no build step. Open it from disk or host it anywhere.
- The regex engine (parser, Thompson NFA, subset construction, minimization) is hand-written; the browser's `RegExp` is used only by the self-tests.
- Press `?` in the app for keyboard shortcuts, the supported grammar and the built-in self-tests.
