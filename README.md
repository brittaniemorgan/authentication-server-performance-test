# Authentication Server Performance Test
Install dependencies with `npm install`
Run with `npm start`

This service exposes two endpoints:

* GET /authenticate
If the provided username and password are the same, returns status (200 OK) and a JSON response with `userId` and `sessionToken`.

* GET /session/keep-alive
If the session exists, echos back the provided `sessionToken` with a (200 OK) response code.

These endpoints are validated using scenarios and stress tested to assess performance.
