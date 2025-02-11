### Gaianet 2 device 
VRAM : 24GB


Tested : RTX 3090 & 4090

### Buat folder
```
mkdir -p gaia
```
### Install gaianet dan config
```
curl -sSfL 'https://raw.githubusercontent.com/GaiaNet-AI/gaianet-node/main/install.sh' | bash -s -- --ggmlcuda 12 --base $HOME/gaia
```
```
gaianet init --base $HOME/gaia
```
### Edit Port
```
cd gaia
```
```
nano config.json
```
* Cari bagian port 8080 dan ganti
```
cd ..
```
```
cd gaia-frp
```
```
nano frpc.toml
```
* Edit bagian port 8080 sesuain sama config.json
### Runing
```
gaianet start --base $HOME/gaia
```
### Node Id dan Device Id
```
gaianet info --base $HOME/gaia
```
