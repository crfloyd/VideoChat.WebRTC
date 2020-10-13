# VideoChat.WebRTC

Room ids are automatically generated when navigating to the base path. If you wish to join another user's room, replace room id with their's in the url.

## Installation

1. Restore node modules: `npm i`
2. Start dev server: `npm run devStart`
3. Navigate to `localhost:3000`

## PeerJS

If you wish to run your own PeerJS server:

1. Install the PeerJS node module: `npm i -g peer`
2. Start a PeerJS server on port 3001: `peerjs --port 3001`
3. Update _script.js_ to use the local server when construction a peer:

```javascript
const myPeer = new Peer(undefined, {
    host: '/',
    port: 3001
})
```
