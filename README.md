# skr-canvas-with-twemoji-and-discord-emoji

A fork of node-canvas-with-twemoji for skr-canvas with Discord emoji support.
This is a module that is able to draw emoji on skr-canvas.

## Installation
```shell
$ npm install skr-canvas-with-twemoji-and-discord-emoji
```
[npm](https://www.npmjs.com/package/skr-canvas-with-twemoji-and-discord-emoji)

## Quick Example
```javascript
const { Canvas } = require('skr-canvas');
const { fillTextWithTwemoji } = require('skr-canvas-with-twemoji-and-discord-emoji');

async function main () {
    const canvas = new Canvas(200, 200);
    const context = canvas.getContext('2d');

    context.fillStyle = '#000000';
    context.font = '30px Arial';
    await fillTextWithTwemoji(context, 'emoji 😉 discord emoji <:id:name>', 100, 100);
}

main();
```

## Dependencies

- skr-canvas [GitHub](https://github.com/samizdatco/skr-canvas)
- twemoji-parser [GitHub](https://github.com/twitter/twemoji-parser)

## License

### skr-canvas-with-twemoji

Copyright (c) 2020-2021 cagpie / Shun Kobayashi <cagpie@gmail.com>

Code licensed under the MIT License: http://opensource.org/licenses/MIT
