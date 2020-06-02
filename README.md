# Integrating HTML5 Games with Playbasis Gamification Platform

## Available States

`Accessed`

`Played`

## Available APIs

`PBSDK.setAccessedGameState(game);`

`PBSDK.setPlayedGameState(game, score);`

## SDK for javascript

```
https://jscdn.pbapp.net/sdk.min.js
```

## Setup JS Library

FILE: index.html

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
  </head>
  <body>
    <button onclick="setAccessedGameState('MyGame')">
      Set AccessedGame state
    </button>
    <button onclick="setPlayedGameState('MyGame', 200)">
      Set PlayedGame state
    </button>

    <!-- load Playbasis HTML5 game integration SDK -->
    <script src="https://jscdn.pbapp.net/sdk.min.js"></script>

    <script src="yourHTML5Game.js"></script>
  </body>
</html>
```

FILE: yourHTML5Game.js

```
function setAccessedGameState(game) {
  PBSDK.setAccessedGameState(game);
}

function setPlayedGameState(game, score) {
  PBSDK.setPlayedGameState(game, score);
}
```

## URL Parameters that need to be sent by Playbasis apps

```
https://YOUR_GAME
?token=TOKEN
&playerId=PLAYER_ID
&playerName=PLAYER_NAME
&playerImage=PLAYER_IMAGE
&socketEndpoint=SOCKET_ENDPOINT
&apiEndpoint=API_ENDPOINT
&campaign_name=CAMPAIGN_NAME
&cid=CID
&sid=SID
```

Please contact Playbasis representative for your test account
or contact support@playbasis.com
