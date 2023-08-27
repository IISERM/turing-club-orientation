1. Install pandoc, make sure it's the latest version. The last time we did it, `apt` installed some archaic version that messed things up.
2. Clone this repository using `git clone --recurse-submodules git@github.com:IISERM/turing-club-orientation.git`
3. `cd` to `turing-club-orientation`.
4. Run `git submodule update --remote --recursive`.
5. Edit `orientation.md`.
6. Run `pandoc -i orientation.md -t revealjs -o index.html --slide-level=2 --standalone -V revealjs-url=./reveal.js`
7. Open `index.html` to view the slides.
8. Run `git commit -m "Update for 20xx orientation" -a`.

Note:- These instructions are suited for deployment to github pages. If you need a standalone version of `index.html` that you can carry around with yourself in a USB, run `pandoc -i orientation.md -t revealjs -o index.html --slide-level=2 --embed-resources -V revealjs-url=./reveal.js` in step 6.

You can find this presentation [here](https://iiserm.github.io/turing-club-orientation/)
