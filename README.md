# Notecast

**Notecast** is a simple utility for transcribing audio files and generating a conspect.

- Requires Python 3.12 (managed by `uv`)
- Needs FFmpeg available in your `PATH`
- Optional: NVIDIA CUDA Toolkit 12.4 for GPU acceleration

## Setup with uv

1. Ensure `uv` is installed: `pip install uv`
2. Install dependencies (creates `.venv`): `uv sync`
3. Run the app: `uv run python main.py`

### CUDA wheels

If you want CUDA wheels from PyTorch, install them after `uv sync`:

```
uv pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu124
```