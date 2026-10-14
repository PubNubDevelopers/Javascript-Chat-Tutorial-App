# JavaScript Chat Tutorial App

Code for the PubNub tutorial [Build a JavaScript chat app with PubNub](https://www.pubnub.com/tutorials/javascript-sdk-chat-app/): a browser chat in plain HTML and JavaScript, with no build step and no server.

Tested with the PubNub JavaScript SDK 13.1.2 (October 2026).

| Folder | Adds |
|---|---|
| `Step 1 - Chat Layout` | Page layout, no chat logic |
| `Step 2 - Basic Chat` | PubNub client, channel subscription, publish and receive messages |
| `Step 3 - Add User Presence` | Live count of online users (Presence) |
| `Step 4 - Add Message Persistence` | Last 10 messages on load (Message Persistence) |
| `Step 5 - Add Usernames` | Display names stored in App Context, updated live with a Signal on `chat-signals` |
| `Step 6 - Message Timestamps` | Send time on every message |

The root `index.html` is the finished app (Step 6).

## Keys

Replace `YOUR_PUBLISH_KEY` and `YOUR_SUBSCRIBE_KEY` in `index.html` with keys from a keyset that has:

- **Presence** tracking events on all channels, or a Presence Management rule for `chat-channel` (step 3). New keysets track presence on selected channels only.
- **Message Persistence** on (step 4). It's on by default.
- **App Context** on (step 5). It's off by default.

## Run

Open `index.html` in two browser tabs, or serve the folder: `python3 -m http.server 8000` and go to `http://localhost:8000/`.
