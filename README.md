# XMRig-Nevo

<sub><sup>Forked from: **[xmrig/xmrig#v6.20.0](https://github.com/xmrig/xmrig)**</sup></sub>

- Use it only for the nevo algorithm: **rx/nevo**
- Pool: **[nevocoin.ch](https://www.nevocoin.ch)**

## Download
- Linux: https://github.com/kryfi-com/xmrig-nevo/releases/download/v6.20.0/xmrig-linux.tar.gz
- MacOS:
  - x64 (Intel): https://github.com/kryfi-com/xmrig-nevo/releases/download/v6.20.0/xmrig-v6.20.0-mac.tar.gz
  - arm64 (M1/M2/M3...): https://github.com/kryfi-com/xmrig-nevo/releases/download/v6.20.0/xmrig-v6.20.0-mac-arm64.tar.gz
- Windows: https://github.com/kryfi-com/xmrig-nevo/releases/download/v6.20.0/xmrig-v6.20.0-win64.zip

For HiveOS, check here: https://github.com/kryfi-com/xmrig-hiveos

## Instructions

### Windows:
- Download the miner: https://github.com/kryfi-com/xmrig-nevo/releases/download/v6.20.0/xmrig-v6.20.0-win64.zip
- Unzip the folder
- Open and modify the `config.json` file at `line 69` with your address: `"user": "YOUR_WALLET_ADDRESS"`
- Run the miner: `xmrig.exe`

### Linux:
- Download the miner:
```bash
wget https://github.com/kryfi-com/xmrig-nevo/releases/download/v6.20.0/xmrig-linux.tar.gz
```

- Extract the archive:
```bash
tar -xf ./xmrig-linux.tar.gz
```

- Enter the miner folder:
```bash
cd ./xmrig
```

- Set the configuration with your own wallet address:
```bash
echo '
{
    "pools": [
        {
            "algo": "rx/nevo",
            "coin": null,
            "url": "nevocoin.ch:2052",
            "user": "YOUR_ADDRESS",
            "pass": "YOUR_WORKER_NAME"
        }
    ]
}
' > config.json
```

- Set execution permission on the miner:
```bash
chmod 701 ./xmrig
```

- Start the miner:
```bash
./xmrig
```
