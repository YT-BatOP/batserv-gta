# BatServ
##### Vous permet d’interroger facilement les serveurs FiveM avec BatServ.

## Installation:
`npm install batserv-gta`

## Utilisation:

```javascript
const batserv = require('batserv-gta')

batserv.query("127.0.0.1", 30120, (err, data) => {
  if (!err) {
    console.log(data)
  } else {
    console.log('Serveur hors ligne.')
  }
})
```

### Sortie:

```javascript
{ maxclients: 64,
  clients: 0,
  challenge: 'xxx',
  gamename: 'GTA5',
  protocol: 4,
  hostname: 'Serveur de Test BatServ',
  gametype: 'Freeroam',
  mapname: 'fivem-map-skater',
  iv: -1698153411 }
```
