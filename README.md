# Fooocus + Indian Style Lora(NSFW) Setup

This README provides step-by-step guidance to run the [Fooocus](https://github.com/lllyasviel/Fooocus) AI image generation tool with the **Indian Style Lora(NSFW)** model.

---

## 📋 What You’ll Need

- Python environment (like Google Colab or Jupyter)
- Internet access for cloning and downloading
- Recommended: Colab Pro or system with high VRAM

---

## 🧰 Setup Overview

1. Install the required Python package (`pygit2`) to handle Git-based operations.
2. Clone the Fooocus repository from GitHub.
3. Navigate to the Fooocus directory.
4. Download the **Indian Style Lora(NSFW)** model file and place it in the appropriate model folder.
5. Launch Fooocus with flags to enable sharing and high VRAM usage.

---

## 📥 Model Details

- **Model Name:** Indian Style Lora(NSFW)
- **Format:** `.safetensors`
- **Source:** [Civitai - Indian Style Lora(NSFW)](https://civitai.com/models/790173/indian-style-loransfw)
- **Purpose:** To generate photorealistic or stylized Indian fashion and portrait images (adult content included)

---

## 🚀 All Commands

```bash
# Step 1: Install required packages
!pip install pygit2==1.15.1

# Step 2: Clone Fooocus repo
%cd /content
!git clone https://github.com/lllyasviel/Fooocus.git
%cd /content/Fooocus

# Step 3: Download the "Indian Style Lora(NSFW)" model
!wget -O /content/Fooocus/models/checkpoints/Indian\ Style\ LoraNsfw.safetensors https://civitai.com/models/790173/indian-style-loransfw

# Step 4: Launch Fooocus
!python entry_with_update.py --share --always-high-vram
