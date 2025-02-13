# Unhandled 'error' event in Node.js HTTP server

This repository demonstrates a common but often overlooked error in Node.js: unhandled 'error' events in HTTP servers.  The provided `bug.js` file showcases a server vulnerable to crashing without informative error messages.

The `bugSolution.js` file provides a solution that handles potential errors gracefully, preventing unexpected server shutdowns and providing more helpful debugging information.

## How to reproduce the bug
1. Clone the repository
2. Run `node bug.js`
3. Observe the server starts, but abruptly exits when an error occurs (e.g. network interruption)
4. Run `node bugSolution.js` and try to trigger the error again. You'll see the server handles error much better.