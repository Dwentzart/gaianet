### Gaianet 2 device 
VRAM : 24GB


Tested : RTX 3090 & 4090 VRAM 24GB MAX 4 NODE

### Buat folder
```
mkdir -p gaia
```
### Install gaianet
```
curl -sSfL 'https://raw.githubusercontent.com/GaiaNet-AI/gaianet-node/main/install.sh' | bash -s -- --ggmlcuda 12 --base $HOME/gaia
```
```
gaianet init --base $HOME/gaia
```
### Edit Port
```
gaianet config --base $HOME/gaia --port 8101
```

### Runing
```
gaianet start --base $HOME/gaia
```
### Node Id dan Device Id
```
gaianet info --base $HOME/gaia
```
