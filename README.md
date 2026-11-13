# Regex Validator Turing Machine

A single-file, browser-only teaching tool: one fixed Turing machine whose language is the set of well-formed regular expressions. Write any string on the tape and the machine steps to ACCEPT or REJECT, with the reason. The 27-state graph is drawn in 3D.

**Live:** https://jonatcompsage.github.io/RegexTuringTest/

- Everything is in `index.html`; there is no build step. Three.js is loaded from cdnjs for the 3D view; without it the Table view shows the same machine.
- Pass 1 sweeps right and checks everything a finite memory can check. Pass 2 zigzags and pairs the parentheses by marking the tape, which is the part a finite automaton cannot do.
- Press `?` in the app for the grammar, how to read the graph, and the built-in self-tests (the machine is compared with a separate recursive-descent recognizer).
- `regex-to-machine.html` is the earlier simulator, which compiles one pattern into its own machine.
