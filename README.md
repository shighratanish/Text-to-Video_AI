#Text-to-Video AI Generator

This project generates a complete video from a simple text description using AI. It combines image generation, speech synthesis, and video processing into a single pipeline.

#Features

- Convert text prompts into AI-generated visuals  
- Automatic voiceover using text-to-speech  
- Dynamic subtitle generation synced with audio  
- Fully automated video creation pipeline  
- GPU-accelerated image generation using Stable Diffusion  

---

#Tech Stack

- PyTorch – Deep learning framework  
- RunwayML Stable Diffusion (v1.5) – Image generation  
- Diffusers (HuggingFace) – Model integration  
- gTTS (Google Text-to-Speech) – Audio generation  
- MoviePy – Video creation & editing  
- Pydub – Audio processing  
- PIL & OpenCV – Image processing  

---

#How It Works

1. User inputs:
   - Text description  
   - Total video duration  
   - Number of frames (images)

2. The system:
   - Generates images using Stable Diffusion  
   - Converts text into speech (voiceover)  
   - Creates a video sequence from generated images  
   - Synchronizes subtitles based on speech timing  
   - Merges everything into a final video  

#Output

- `images/` → Generated frames  
- `voiceover.mp3` → Audio narration  
- `final_video.mp4` → Final AI-generated video  

#▶️ Usage

Run the script and provide:

Enter the video description  
Enter total duration (seconds)  
Enter number of images  

The system will automatically generate and download the final video.

#🖥️ Requirements

- Python 3.8+  
- CUDA-enabled GPU (recommended)  
- Google Colab / Local GPU setup  

Install dependencies:

```bash
pip install torch torchvision torchaudio
pip install diffusers transformers accelerate
pip install moviepy gtts pydub opencv-python numpy
