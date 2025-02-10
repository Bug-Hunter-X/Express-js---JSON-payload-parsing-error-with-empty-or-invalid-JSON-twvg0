# Express.js JSON Payload Parsing Issue

This repository demonstrates a common issue in Express.js applications where parsing JSON payloads from POST requests fails when the request body is empty or contains invalid JSON data.  The problem stems from the `express.json()` middleware's behavior when it encounters malformed input.  This can lead to unexpected errors and prevent the application from properly handling requests.

## Bug Description
The provided `bug.js` file shows an Express.js server that attempts to parse the JSON body of POST requests to `/data`. If the request body is empty or contains invalid JSON, the server will not correctly handle the request, potentially leading to errors or unexpected behavior. 

## Solution
The `bugSolution.js` file demonstrates a solution to this problem by adding error handling to gracefully manage situations where the request body is invalid.