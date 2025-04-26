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
### Install config qwen 2.5 0.5b
```
gaianet init --config https://raw.githubusercontent.com/GaiaNet-AI/node-configs/main/qwen2.5-0.5b-instruct/config.json
```
```
gaianet init --base $HOME/gaia
```
### Edit Port
```
gaianet config --base $HOME/gaia --port 8101
```
```
gaianet config --base $HOME/gaian --port 8102
```
```
gaianet config --base $HOME/gaiann --port 8103
```
```
gaianet config --base $HOME/gaians --port 8104
```


### Runing
```
gaianet start --base $HOME/gaia
```
### Node Id dan Device Id
```
gaianet info --base $HOME/gaia
```
