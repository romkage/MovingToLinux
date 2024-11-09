# Lutris

## Game Info

### Runner
Wine

## Game Options

### Working directory

Point to directory containing the already installed game.

eg.
```
Working directory: /home/romkage/apps/The Great Game/TheGreatGame.exe
```

### Wine Prefix

Find a wine prefix (a wine dir) previously created by a steam game. You could do it like so:
```
find /home -type d -path "*/.local/share/Steam/steamapps/compatdata/*/pfx" 2>/dev/null
```

and add that to wineprefix.

Eg.
```
/home/romkage/.var/app/com.valvesoftware.Steam/.local/share/Steam/steamapps/compatdata/1234567/pfx
```

### Prefix Architecture

I've read that auto doesnt always work, so you may have to set it it match. I just picked 64bit.


## Runner Options

### Wine version

Proton. Eg proton experimental.

### Direct 3D.

I got an error that direct 3d wasnt installed. I read that i should put an enviroment variable called: `PROTON_USE_WINED3D` set equal to `1`.

but i put, by accident under the `Runner Options` tab -> DLL overrides, because it looks similar. ANd then the game started up fine. Even more weird, removing it again, the game still starts fine. So i dont know :/.
