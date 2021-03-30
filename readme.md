## Node Tests

This is a simple repo with a couple of tests of some node scripts. The first one works, but the other 3 fail.

1. foo.js really simple script
2. babel
3. gatsby
4. next

### foo.js

1. run `RECORD_REPLAY_DRIVER=./macOS-recordreplay.so RECORD_REPLAY_DISPATCH=wss://dispatch.replay.io RECORD_REPLAY_RECORDING_ID_FILE=./recordings.log ./macOS-replay-node foo.js`
2. check `recordings.log` and go to `https://replay.io/view?id=<id>`

### babel

1. `npm i`
2. run `RECORD_REPLAY_DRIVER=./macOS-recordreplay.so RECORD_REPLAY_DISPATCH=wss://dispatch.replay.io RECORD_REPLAY_RECORDING_ID_FILE=./recordings.log ./macOS-replay-node ./node_modules/.bin/babel src -d lib`
3. check `recordings.log` and go to `https://replay.io/view?id=<id>`

### Gatsby

1. `cd my-gatsby-site`
2. `npm i`
3. run `RECORD_REPLAY_DRIVER=../macOS-recordreplay.so RECORD_REPLAY_DISPATCH=wss://dispatch.replay.io RECORD_REPLAY_RECORDING_ID_FILE=../recordings.log ../macOS-replay-node ./node_modules/.bin/gatsby build`
4. check `../recordings.log` and go to `https://replay.io/view?id=<id>`

### Next

1. `cd my-next-app`
2. `npm i`
3. run `RECORD_REPLAY_DRIVER=../macOS-recordreplay.so RECORD_REPLAY_DISPATCH=wss://dispatch.replay.io RECORD_REPLAY_RECORDING_ID_FILE=../recordings.log ../macOS-replay-node ./node_modules/.bin/next build`
4. check `../recordings.log` and go to `https://replay.io/view?id=<id>`
