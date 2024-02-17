# horde-bridge-lcpp-server

A really simple proof of concept that bridges requests from the [AI
Horde](https://aihorde.net/) to
[llama.cpp](https://github.com/ggerganov/llama.cpp)'s
[server](https://github.com/ggerganov/llama.cpp/tree/master/examples/server).

Released under the Apache License, version 2.0.

# Quickstart guide

```
git clone https://github.com/Artefact2/horde-bridge-lcpp-server
cd horde-bridge-lcpp-server

git clone https://github.com/ggerganov/llama.cpp
make -C llama.cpp LLAMA_HIPBLAS=1 AMDGPU_TARGETS=gfx1030 server # tweak build type to your hardware

cp config.json.example config.json
$EDITOR config.json
./bridge
```
