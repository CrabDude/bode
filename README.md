# `bode`

Like [`babel-node`](https://babeljs.io/docs/usage/cli/), except using [`babel-register`](https://babeljs.io/docs/usage/require/) so `--debug-brk` breaks on the actual first line of code, not babel-node's first line of code:

## Install

```bash
npm install -g bode
```
## Use

Use it transparently like `node` to debug using [`--inspect`](https://medium.com/@paul_irish/debugging-node-js-nightlies-with-chrome-devtools-7c4a1b95ae27#.ntu7ibdek) in v6.4+:

```bash
# breaks on first line of foo.js
bode --inspect --debug-brk foo.js
```
