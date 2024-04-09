# rainlink-deezer
A rainlink plugin that allows you to play music on deezer

Install
```
npm i rainlink-deezer
```

Support source:
```
- https://www.deezer.com/us/playlist/53362031
- https://www.deezer.com/us/track/6745599
- https://www.deezer.com/us/album/103248
```
How to
```js
const { Rainlink } = require('rainlink');
const { DeezerPlugin } = require('rainlink-deezer');

const rainlink = new Rainlink({
    library: new Library.DiscordJS(client),
    nodes: Nodes,
    plugins: [
      new DeezerPlugin(),
    ],
});
rainlink.search(`https://www.deezer.com/us/playlist/53362031`); // track, album, playlist
rainlink.search('mirror heart', { engine: 'deezer' }); // search track using deezer
```