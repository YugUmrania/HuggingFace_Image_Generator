# HuggingFace Image Generator

A simple CLI tool that generates images from text prompts using the Hugging Face Inference API (FLUX.1-schnell model).

## Features

- Generates images from any text prompt
- Uses the `black-forest-labs/FLUX.1-schnell` model via `fal-ai` provider
- Saves the result as `generated_image.png`

## Requirements

- Python 3.8+
- A Hugging Face account and access token ([Get one here](https://huggingface.co/settings/tokens))

## Installation

1. Clone the repository:
   ```bash
   git clone <repo-url>
   cd HuggingFace_Image_Generator
   ```

2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   venv\Scripts\activate   # Windows
   source venv/bin/activate   # macOS/Linux
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set your Hugging Face token as an environment variable:
   ```bash
   set HF_TOKEN=your_hf_token   # Windows
   export HF_TOKEN=your_hf_token   # macOS/Linux
   ```

## Usage

Run the script and enter your prompt when asked:

```bash
python image_generation.py
```

The generated image will be saved as `generated_image.png` in the current directory.

## Notes

- The `HF_TOKEN` environment variable is required; set it before running the script.
- Generation requires an internet connection and uses Hugging Face inference credits.