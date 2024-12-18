---
license: apache-2.0
base_model: hooking-dev/sexyGPT-Uncensored
tags:
- TensorBlock
- GGUF
---

<div style="width: auto; margin-left: auto; margin-right: auto">
<img src="https://i.imgur.com/jC7kdl8.jpeg" alt="TensorBlock" style="width: 100%; min-width: 400px; display: block; margin: auto;">
</div>
<div style="display: flex; justify-content: space-between; width: 100%;">
    <div style="display: flex; flex-direction: column; align-items: flex-start;">
        <p style="margin-top: 0.5em; margin-bottom: 0em;">
            Feedback and support: TensorBlock's  <a href="https://x.com/tensorblock_aoi">Twitter/X</a>, <a href="https://t.me/TensorBlock">Telegram Group</a> and <a href="https://x.com/tensorblock_aoi">Discord server</a>
        </p>
    </div>
</div>

## hooking-dev/sexyGPT-Uncensored - GGUF

This repo contains GGUF format model files for [hooking-dev/sexyGPT-Uncensored](https://huggingface.co/hooking-dev/sexyGPT-Uncensored).

The files were quantized using machines provided by [TensorBlock](https://tensorblock.co/), and they are compatible with llama.cpp as of [commit b4242](https://github.com/ggerganov/llama.cpp/commit/a6744e43e80f4be6398fc7733a01642c846dce1d).

<div style="text-align: left; margin: 20px 0;">
    <a href="https://tensorblock.co/waitlist/client" style="display: inline-block; padding: 10px 20px; background-color: #007bff; color: white; text-decoration: none; border-radius: 5px; font-weight: bold;">
        Run them on the TensorBlock client using your local machine ↗
    </a>
</div>

## Prompt template

```

```

## Model file specification

| Filename | Quant type | File Size | Description |
| -------- | ---------- | --------- | ----------- |
| [sexyGPT-Uncensored-Q2_K.gguf](https://huggingface.co/tensorblock/sexyGPT-Uncensored-GGUF/blob/main/sexyGPT-Uncensored-Q2_K.gguf) | Q2_K | 0.081 GB | smallest, significant quality loss - not recommended for most purposes |
| [sexyGPT-Uncensored-Q3_K_S.gguf](https://huggingface.co/tensorblock/sexyGPT-Uncensored-GGUF/blob/main/sexyGPT-Uncensored-Q3_K_S.gguf) | Q3_K_S | 0.090 GB | very small, high quality loss |
| [sexyGPT-Uncensored-Q3_K_M.gguf](https://huggingface.co/tensorblock/sexyGPT-Uncensored-GGUF/blob/main/sexyGPT-Uncensored-Q3_K_M.gguf) | Q3_K_M | 0.098 GB | very small, high quality loss |
| [sexyGPT-Uncensored-Q3_K_L.gguf](https://huggingface.co/tensorblock/sexyGPT-Uncensored-GGUF/blob/main/sexyGPT-Uncensored-Q3_K_L.gguf) | Q3_K_L | 0.102 GB | small, substantial quality loss |
| [sexyGPT-Uncensored-Q4_0.gguf](https://huggingface.co/tensorblock/sexyGPT-Uncensored-GGUF/blob/main/sexyGPT-Uncensored-Q4_0.gguf) | Q4_0 | 0.107 GB | legacy; small, very high quality loss - prefer using Q3_K_M |
| [sexyGPT-Uncensored-Q4_K_S.gguf](https://huggingface.co/tensorblock/sexyGPT-Uncensored-GGUF/blob/main/sexyGPT-Uncensored-Q4_K_S.gguf) | Q4_K_S | 0.107 GB | small, greater quality loss |
| [sexyGPT-Uncensored-Q4_K_M.gguf](https://huggingface.co/tensorblock/sexyGPT-Uncensored-GGUF/blob/main/sexyGPT-Uncensored-Q4_K_M.gguf) | Q4_K_M | 0.113 GB | medium, balanced quality - recommended |
| [sexyGPT-Uncensored-Q5_0.gguf](https://huggingface.co/tensorblock/sexyGPT-Uncensored-GGUF/blob/main/sexyGPT-Uncensored-Q5_0.gguf) | Q5_0 | 0.122 GB | legacy; medium, balanced quality - prefer using Q4_K_M |
| [sexyGPT-Uncensored-Q5_K_S.gguf](https://huggingface.co/tensorblock/sexyGPT-Uncensored-GGUF/blob/main/sexyGPT-Uncensored-Q5_K_S.gguf) | Q5_K_S | 0.122 GB | large, low quality loss - recommended |
| [sexyGPT-Uncensored-Q5_K_M.gguf](https://huggingface.co/tensorblock/sexyGPT-Uncensored-GGUF/blob/main/sexyGPT-Uncensored-Q5_K_M.gguf) | Q5_K_M | 0.127 GB | large, very low quality loss - recommended |
| [sexyGPT-Uncensored-Q6_K.gguf](https://huggingface.co/tensorblock/sexyGPT-Uncensored-GGUF/blob/main/sexyGPT-Uncensored-Q6_K.gguf) | Q6_K | 0.138 GB | very large, extremely low quality loss |
| [sexyGPT-Uncensored-Q8_0.gguf](https://huggingface.co/tensorblock/sexyGPT-Uncensored-GGUF/blob/main/sexyGPT-Uncensored-Q8_0.gguf) | Q8_0 | 0.178 GB | very large, extremely low quality loss - not recommended |


## Downloading instruction

### Command line

Firstly, install Huggingface Client

```shell
pip install -U "huggingface_hub[cli]"
```

Then, downoad the individual model file the a local directory

```shell
huggingface-cli download tensorblock/sexyGPT-Uncensored-GGUF --include "sexyGPT-Uncensored-Q2_K.gguf" --local-dir MY_LOCAL_DIR
```

If you wanna download multiple model files with a pattern (e.g., `*Q4_K*gguf`), you can try:

```shell
huggingface-cli download tensorblock/sexyGPT-Uncensored-GGUF --local-dir MY_LOCAL_DIR --local-dir-use-symlinks False --include='*Q4_K*gguf'
```
