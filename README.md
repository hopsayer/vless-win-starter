# VLESS Windows Starter

Simple one-click VLESS proxy starter for Windows using sing-box.

## Features

- One-button proxy enable/disable
- Minimal configuration
- Most compatible version (1.9.7) of most modern proxy engine (sing-box), downloaded automatically on first run
- AK47-like - simple and reliable

## Requirements

- Windows 10 or newer
- Internet connection for first run (obviously)

## Needed folder structure

```
vless-win-starter-simple/
├── prepare-and-start.bat
└── config.json (filled-in config-template.json)
```

## What to do

1. Download this repository or just files separately: config-template.json and prepare-and-start.bat
2. Rename `config-template.json` to `config.json`
3. Fill `config.json` with your server details:
```
     Get your VLESS key. Usually you have VLESS subscription link starting with `https://`. Open it. There you will have your VLESS key starting with (`vless://...`). Paramenters you need are inside of it. 
     Fill your `config.json` with them accordingly:

       `server` - your server address
       `server_port` - your server port
       `uuid` - your UUID
       `public_key` - Reality public key
       `short_id` - Reality short ID
       `server_name` - SNI (e.g., www.microsoft.com)
```

```
The other way is to import your VLESS subscription link into Nekoray (can be downloaded here: https://github.com/MatsuriDayo/nekoray/releases/download/4.0.1/nekoray-4.0.1-2024-12-12-windows64.zip) and then export VLESS key from it (Share > Export sing-box config (Ctrl+E)). You will get config.json too, but not so manually. 
```

4. Run `prepare-and-start.bat`, preferably as Admin

![GitHub views](https://komarev.com/ghpvc/?username=hopsayer&repo=vless-win-starter-simple&color=green&style=flat-square)
