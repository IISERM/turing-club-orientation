1. Install pandoc, make sure it's the latest version. The last time we did it, `apt` installed some archaic version that messed things up.
2. Clone this repository using `git clone --recurse-submodules git@github.com:IISERM/turing-club-orientation.git`
3. `cd` to `turing-club-orientation`.
4. Run `git submodule update --remote --recursive`.
5. Edit `orientation.md`.
6. Run `pandoc -i orientation.md -t revealjs -o index.html --slide-level=2 --standalone -V revealjs-url=./reveal.js`