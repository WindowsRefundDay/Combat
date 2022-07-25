# Combat 360
DEFEAT WAKE COUNTY WITH INCOGNITO!!!

# Setup (for debian based distros)
```
git clone https://github.com/WindowsRefundDay/Combat-360.git
cd Incognito
git submodule update --init
```

## Config

```json
{
    "port": 8080,
    "ssl": false,
    "prefix": "/service/",
    "codec": "xor",
    "proxy": true,
    "blacklist": [],
    "addresses": [],
    "authorization": {
        "name": "__incog_auth",
        "value": "1"
    },
    "appearance": "bright",
    "engine": "google"
}
```

- `port` HTTP Server Port
- `ssl` (true / false) HTTP Server SSL
- `prefix` Corrosion proxy prefix
- `codec` Corrosion proxy codec
- `proxy` (true / false) Have Corrosion be hosted on the Node.js application. Recommended to have Corrosion hosted elsewhere with large amounts of clients.
- `blacklist` Array of hostnames to be blocked on the proxy.
- `authorization` (Object { name: "...", value: "..." } / false) Proxy authorization cookie
- `appearance` ("bright" / "midnight" / "ocean" / "lime" / "terminal") Default site appearance
- `engine` ("google" / "bing" / "brave" / "youtube" / "twitter" / "reddit") Default search engine 


# Ultraviolet
Ultraviolet's bare server by default is set to Incognito's official bare server (https://incog.dev/bare/)

Change the bare server in `uv/uv.config.js` to whatever bare server you have.

Folder prefixes in `uv.sw.js` and `uv.config.js` will have to be changed to where `uv/` is located

`/uv.sw.js` --> `/uv/uv.sw.js`

# Games
Games are not included by default due to the extremely large size of them. They need to be put in the games folder

```
git clone https://github.com/caracal-js/gfiles.git source
```
