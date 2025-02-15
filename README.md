# Node.js Server Hang - Synchronous Operation

This repository demonstrates a common issue in Node.js applications: a server hanging due to a long-running synchronous operation that blocks the event loop. The `bug.js` file contains code that simulates this scenario.  The solution is shown in `bugSolution.js`.

## Problem

The server performs a time-consuming task synchronously within the request handler. This prevents the event loop from processing other requests and leads to the server becoming unresponsive.