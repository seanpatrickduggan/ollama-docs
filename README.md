# ollama-docs

## Make sure git-lfs is installed (https://git-lfs.com)
```
git lfs install
git clone https://huggingface.co/Qwen/Qwen2.5-Coder-14B
```
## Importing a model from Safetensors weights
First, create a Modelfile with a FROM command which points to the directory containing your Safetensors weights:
```
FROM /path/to/safetensors/directory
```

Then, from the directory
```
ollama create --quantize q4_K_M qwen2.5-coder-14b_q4_K_M
```
