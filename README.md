# BOTC Final Multiplayer

Mobile-first shared-table BOTC web app.

## Deploy from a phone
Upload these files to a GitHub repository:
- package.json
- server.js
- public/index.html
Then deploy the repository to a Node.js host that supports Socket.IO/WebSockets and HTTPS.

## Run
npm install
npm start

## Multiplayer
Rooms and game state are real-time through Socket.IO. Camera/audio uses browser WebRTC mesh signaling with a public STUN server. For reliable production use across restrictive networks, add a TURN server or an SFU; mesh bandwidth grows with player count.

## Security/game rules
This is a gameplay foundation, not an official BOTC rules engine. The Storyteller controls roles, phases and deaths. A production rules engine can be layered onto the same room architecture.
