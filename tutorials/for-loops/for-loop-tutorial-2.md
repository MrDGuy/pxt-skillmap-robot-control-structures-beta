# For Loops

## Introduction @unplugged

In this tutorial you will write a for loop which will repeat 3 times. Each time the loop repeats the robot should move over a hurdle and place a coin in the gap space. The end goal is to fill each gap with a coin on the bottom row before reaching the goal tile.
![Jump Hurdles](https://raw.githubusercontent.com/MrDGuy/pxt-skillmap-robot-control-structures/main/docs/static/robot-cs-for-hurdles.gif "Jump Hurdles" )

## Step One

Using the ``||robot:begin_screen||`` code begin the screen with the hurdle tilemap.

```python
robot.begin_screen()
```

## Step Two

Now click the ``||loops:loops||`` category from the toolbox and drag in the ``||loops:for||`` code to line 2.

```python
robot.begin_screen()
for i in range(4):
    pass
```

## Step Three

Change the 4 inside the paretheses to a 3 since there are only 3 gaps to place a coin.

```python
robot.begin_screen()
for i in range(3):
    pass
```

## Step Four

Write the code you want to repeat to get the robot to move to each gap and "jump" each hurdle.
![Jump Hurdles](https://raw.githubusercontent.com/MrDGuy/pxt-skillmap-robot-control-structures/main/docs/static/robot-cs-for-hurdles.gif "Jump Hurdles" )

```python
robot.begin_screen()
for i in range(3):
    #Your hurdle code here
```

## Step Five

Write the code to move the robot to the goalTile below the for loop but over to the far left margin.

```python
robot.begin_screen()
for i in range(3):
    #Your hurdle code here
#write the code here to move to the goalTile after the hurdles (so it is not included in the loop).


#code for toolbox (don't write these commands).
robot.turn_right()
robot.turn_left()
robot.move_forward()
robot.collect_coin()
robot.place_coin()
def do_something():
    pass
```


```assetjson
{
  "README.md": " ",
  "assets.json": "",
  "main.blocks": "<xml xmlns=\"https://developers.google.com/blockly/xml\"><block type=\"pxt-on-start\" x=\"0\" y=\"0\"></block></xml>",
  "main.py": "",
  "main.ts": "\n",
  "pxt.json": "{\n    \"name\": \"Non Git Hub Robot Assets CS Skillmap For Loop 2\",\n    \"description\": \"\",\n    \"dependencies\": {\n        \"device\": \"*\",\n        \"tilemaps\": \"github:microsoft/pxt-tilemaps#v1.12.0\",\n        \"Robot Extension\": \"github:MrDGuy/robot-extension-beta#2e0bf1965f09d6a34dd4a81ab5013694fae62cb9\"\n    },\n    \"files\": [\n        \"main.blocks\",\n        \"main.ts\",\n        \"README.md\",\n        \"assets.json\",\n        \"tilemap.g.jres\",\n        \"tilemap.g.ts\",\n        \"main.py\"\n    ],\n    \"targetVersions\": {\n        \"branch\": \"v1.13.31\",\n        \"tag\": \"v1.13.31\",\n        \"commits\": \"https://github.com/microsoft/pxt-arcade/commits/ef3aad740700f5159eebccf721fa35d32683fcaa\",\n        \"target\": \"1.13.31\",\n        \"pxt\": \"9.1.6\"\n    },\n    \"preferredEditor\": \"pyprj\"\n}\n",
  "tilemap.g.jres": "{\n    \"tile1\": {\n        \"data\": \"hwQQABAAAAD//////////09ERERERET0T0RERERERPRPRERERERE9E9ERERERET0T0RERERERPRPRERERERE9E9ERERERET0T0RERERERPRPRERERERE9E9ERERERET0T0RERERERPRPRERERERE9E9ERERERET0T0RERERERPT//////////w==\",\n        \"mimeType\": \"image/x-mkcd-f4\",\n        \"tilemapTile\": true,\n        \"displayName\": \"startTile\"\n    },\n    \"tile2\": {\n        \"data\": \"hwQQABAAAAD//////////4+IiIiIiIj4j4iIiIiIiPiPiIiIiIiI+I+IiIiIiIj4j4iIiIiIiPiPiIiIiIiI+I+IiIiIiIj4j4iIiIiIiPiPiIiIiIiI+I+IiIiIiIj4j4iIiIiIiPiPiIiIiIiI+I+IiIiIiIj4j4iIiIiIiPj//////////w==\",\n        \"mimeType\": \"image/x-mkcd-f4\",\n        \"tilemapTile\": true,\n        \"displayName\": \"goalTile\"\n    },\n    \"tile3\": {\n        \"data\": \"hwQQABAAAAD//////////x8RERERERHxHxEREREREfEfERERERER8R8RERERERHxHxEREREREfEfERERERER8R8RERERERHxHxEREREREfEfERERERER8R8RERERERHxHxEREREREfEfERERERER8R8RERERERHxHxEREREREfH//////////w==\",\n        \"mimeType\": \"image/x-mkcd-f4\",\n        \"tilemapTile\": true,\n        \"displayName\": \"floorTile\"\n    },\n    \"tile4\": {\n        \"data\": \"hwQQABAAAAD//////////393d3d3d3f3f3d3d3d3d/d/d3d3d3d39393d3d3d3f3f3d3d3d3d/d/d3d3d3d39393d3d3d3f3f3d3d3d3d/d/d3d3d3d39393d3d3d3f3f3d3d3d3d/d/d3d3d3d39393d3d3d3f3f3d3d3d3d/f//////////w==\",\n        \"mimeType\": \"image/x-mkcd-f4\",\n        \"tilemapTile\": true,\n        \"displayName\": \"coinTile\"\n    },\n    \"transparency16\": {\n        \"data\": \"hwQQABAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA==\",\n        \"mimeType\": \"image/x-mkcd-f4\",\n        \"tilemapTile\": true\n    },\n    \"tile5\": {\n        \"data\": \"hwQQABAAAAD//////////7+7u7u7u7v7v7u7u7u7u/u/u7u7u7u7+7+7u7u7u7v7v7u7u7u7u/u/u7u7u7u7+7+7u7u7u7v7v7u7u7u7u/u/u7u7u7u7+7+7u7u7u7v7v7u7u7u7u/u/u7u7u7u7+7+7u7u7u7v7v7u7u7u7u/v//////////w==\",\n        \"mimeType\": \"image/x-mkcd-f4\",\n        \"tilemapTile\": true,\n        \"displayName\": \"wallTile\"\n    },\n    \"level2\": {\n        \"id\": \"level2\",\n        \"mimeType\": \"application/mkcd-tilemap\",\n        \"data\": \"MTAwYTAwMDcwMDA0MDUwNTBjMDUwNTBjMDUwNTA2MGEwMzAzMDMwMzAzMDMwMzAyMDcwYTAzMDMwMzAzMDMwMzAzMDMwNzBmMDMwMzAzMDMwMzAzMDMwMzBlMGEwMzAzMDMwMzAzMDMwMzAzMDcwYTAxMTAwMzEwMDMxMDAzMTAwNzA5MGIwYjBkMGIwYjBkMGIwYjA4MjIyMjIyMjIyMjAyMDAwMDAwMjAwMjAwMDAwMDIwMDIwMDAwMDAyMDAyMDAwMDAwMjAwMjAyMDIwMjIyMjIyMjIyMjIyMg==\",\n        \"tileset\": [\n            \"myTiles.transparency16\",\n            \"myTiles.tile1\",\n            \"myTiles.tile2\",\n            \"myTiles.tile3\",\n            \"sprites.dungeon.greenOuterNorthWest\",\n            \"sprites.dungeon.greenOuterNorth0\",\n            \"sprites.dungeon.greenOuterNorthEast\",\n            \"sprites.dungeon.greenOuterEast0\",\n            \"sprites.dungeon.greenOuterSouthWest\",\n            \"sprites.dungeon.greenOuterSouthEast\",\n            \"sprites.dungeon.greenOuterWest0\",\n            \"sprites.dungeon.greenOuterSouth1\",\n            \"sprites.dungeon.greenOuterNorth2\",\n            \"sprites.dungeon.greenOuterSouth2\",\n            \"sprites.dungeon.greenOuterEast2\",\n            \"sprites.dungeon.greenOuterWest2\",\n            \"myTiles.tile5\"\n        ],\n        \"displayName\": \"level1\"\n    },\n    \"*\": {\n        \"mimeType\": \"image/x-mkcd-f4\",\n        \"dataEncoding\": \"base64\",\n        \"namespace\": \"myTiles\"\n    }\n}",
  "tilemap.g.ts": "// Auto-generated code. Do not edit.\nnamespace myTiles {\n    //% fixedInstance jres blockIdentity=images._tile\n    export const tile1 = image.ofBuffer(hex``);\n    //% fixedInstance jres blockIdentity=images._tile\n    export const tile2 = image.ofBuffer(hex``);\n    //% fixedInstance jres blockIdentity=images._tile\n    export const tile3 = image.ofBuffer(hex``);\n    //% fixedInstance jres blockIdentity=images._tile\n    export const tile4 = image.ofBuffer(hex``);\n    //% fixedInstance jres blockIdentity=images._tile\n    export const transparency16 = image.ofBuffer(hex``);\n    //% fixedInstance jres blockIdentity=images._tile\n    export const tile5 = image.ofBuffer(hex``);\n\n    helpers._registerFactory(\"tilemap\", function(name: string) {\n        switch(helpers.stringTrim(name)) {\n            case \"level1\":\n            case \"level2\":return tiles.createTilemap(hex`0a0007000405050c05050c0505060a0303030303030302070a0303030303030303070f03030303030303030e0a0303030303030303070a011003100310031007090b0b0d0b0b0d0b0b08`, img`\n2 2 2 2 2 2 2 2 2 2 \n2 . . . . . . . . 2 \n2 . . . . . . . . 2 \n2 . . . . . . . . 2 \n2 . . . . . . . . 2 \n2 . 2 . 2 . 2 . 2 2 \n2 2 2 2 2 2 2 2 2 2 \n`, [myTiles.transparency16,myTiles.tile1,myTiles.tile2,myTiles.tile3,sprites.dungeon.greenOuterNorthWest,sprites.dungeon.greenOuterNorth0,sprites.dungeon.greenOuterNorthEast,sprites.dungeon.greenOuterEast0,sprites.dungeon.greenOuterSouthWest,sprites.dungeon.greenOuterSouthEast,sprites.dungeon.greenOuterWest0,sprites.dungeon.greenOuterSouth1,sprites.dungeon.greenOuterNorth2,sprites.dungeon.greenOuterSouth2,sprites.dungeon.greenOuterEast2,sprites.dungeon.greenOuterWest2,myTiles.tile5], TileScale.Sixteen);\n        }\n        return null;\n    })\n\n    helpers._registerFactory(\"tile\", function(name: string) {\n        switch(helpers.stringTrim(name)) {\n            case \"startTile\":\n            case \"tile1\":return tile1;\n            case \"goalTile\":\n            case \"tile2\":return tile2;\n            case \"floorTile\":\n            case \"tile3\":return tile3;\n            case \"coinTile\":\n            case \"tile4\":return tile4;\n            case \"transparency16\":return transparency16;\n            case \"wallTile\":\n            case \"tile5\":return tile5;\n        }\n        return null;\n    })\n\n}\n// Auto-generated code. Do not edit.\n"
}
```

```customts
    tiles.loadMap(tiles.createMap(tilemap`level1`))
    robot.beginScreen()
    game.onUpdate(function () {
        if (robot.goalReached()) {
            music.play(music.melodyPlayable(music.powerUp), music.PlaybackMode.UntilDone)
            game.splash("You reached the goal!")
            game.reset()
        }
    })
```
