# PyTorch
Make sure to install PyTorch with the appropriate CUDA version.

```
pip install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu128 -U
```

# Fairseq

I'm not sure how or why I installed fairseq back in the day, but probably it was this one.

https://github.com/One-sixth/fairseq/releases

```
pip install fairseq-0.12.3-cp311-cp311-win_amd64.whl
```
SHA256: 6a10ed5bf617dd4dcd7bfc4506ffa9d58c30e2b81b81050b2448578a034f7f72

[There are also other versions](https://huggingface.co/Jmica/rvc/tree/main)

# Matplotlib

```
AttributeError: 'FigureCanvasAgg' object has no attribute 'tostring_rgb'
```

The `tostring_rgb` function was removed in newer versions.
Downgrade to a compatible version:

```
pip install matplotlib==3.9.0
```

# Gradio

```
"Cannot import name 'media_data' from 'gradio_client'" and "TypeError: Blocks.queue() got an unexpected keyword argument 'concurrency_count'"
```

[Issue](https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI/issues/2737#issuecomment-3758330496)

```
pip install gradio-client==0.2.10
pip install gradio==3.48.0
```