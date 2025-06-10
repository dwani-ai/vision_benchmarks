Setup Benchmarks


Add - daemon.json to /etc/docker/
- sudo systemctl restart docker

sudo docker run --runtime nvidia -it --rm -p 7881:8000 slabstech/dwani-vllm

export HF_TOKEN='some_Read_token'

export VLLM_CONFIGURE_LOGGING=0

 vllm serve Qwen/Qwen3-0.6B --served-model-name qwen3  --disable-log-requests --uvicorn-log-level=warning

  vllm serve google/gemma-3-1b-it --served-model-name gemma3  --disable-log-requests --uvicorn-log-level=warning

  vllm serve google/gemma-3-4b-it --served-model-name gemma3  --disable-log-requests --uvicorn-log-level=warning


  vllm serve google/gemma-3-12b-it --served-model-name gemma3  --disable-log-requests --uvicorn-log-level=warning

