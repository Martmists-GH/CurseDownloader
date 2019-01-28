# CurseDownloader

Download mod information from CurseForge to create an easy manifest.json


## Configuration

### config.json

```json
{
  "author": "Your name",
  "forge": "Specific forge version, e.g. 14.23.5.2808",
  "pack": "Modpack name",
  "version": "Pack version number"
}

```


### mods.txt

```
# Minecraft [minecraft version, e.g. 1.12]
mod-one
mod-two
mod-three
```

The format these mods must be in is the name in the URL on CurseForge, like so:

```
Ender IO -> ender-io
Thermal Expansion -> thermalexpansion
Just Enough Items -> jei
Astral Sorcery -> astral-sorcery
```


## Generating manifest.json

After configuring these files, you should be able to just run this:

```bash
$ python -m pip install -r requirements.txt
$ python main.py
```
