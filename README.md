# 📰 AI Video Generator

## 📖 Introduction
AI Video Generator is a Python-based automation tool designed to transform the latest trending news articles into visually rich, ready-to-publish videos.  
It works by automatically fetching current news headlines and summaries, generating narration using text-to-speech, creating graphic text overlays, and combining them with relevant background images to produce short video segments.  

The goal of this project is to save time for content creators, news publishers, and social media managers by automating the repetitive work of news video creation.  
Instead of manually recording narration, searching for background visuals, and editing videos, this tool completes the entire process in a few minutes.

This type of automation can be used for:
- Short-form news reels for platforms like Instagram, YouTube Shorts, and TikTok
- Breaking news alerts on social media
- Daily news digests for websites or blogs
- Quick summaries of events for internal communications

---

## ✨ How It Works
The system follows a straightforward pipeline:

1. **News Collection** – Uses the Google News RSS feed to retrieve current trending stories, extracting both headlines and summaries.
2. **Image Retrieval** – Connects to the Unsplash Source API to find high-quality images related to the news topic.
3. **Narration Creation** – Generates natural-sounding audio narration of the news script using Google Text-to-Speech (gTTS).
4. **Overlay Generation** – Creates a transparent text overlay image with the headline and summary using the Pillow image processing library.
5. **Video Composition** – Combines the background image, text overlay, and narration into a single video using MoviePy and FFmpeg.
6. **Export** – Saves the final video to the project directory, ready for sharing or publishing.

---

## 🛠️ Technology Stack

| Component              | Tools and Libraries |
|------------------------|---------------------|
| Data Retrieval         | requests, beautifulsoup4 |
| Text-to-Speech         | gTTS |
| Image Processing       | Pillow (PIL) |
| Video Editing          | MoviePy |
| Audio Processing       | pydub |
| Image Sourcing         | Unsplash Source API |
| Video/Audio Handling   | ffmpeg |
| Font Rendering         | fonts-dejavu |

---

## 📂 Project Structure
```
AI-Video-Generator/
│── AI_video_generating_tool_py.ipynb  # Main Jupyter Notebook
│── requirements.txt                   # Dependencies
│── README.md                           # Documentation
```

---

## ⚡ Installation

1. Clone the repository to your system:
   ```bash
   git clone https://github.com/AdityaGaur19/AI-Video-Generator.git
   cd AI-Video-Generator
   ```

2. Install required Python dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Install FFmpeg, which is required for video and audio processing.  
   Follow the official installation guide: [https://ffmpeg.org/download.html](https://ffmpeg.org/download.html)

---

## 🚀 Usage Guide

1. Open the Jupyter Notebook file:
   ```bash
   jupyter notebook AI_video_generating_tool_py.ipynb
   ```

2. Run the cells in sequence to:
   - Retrieve the latest news from Google News RSS feed
   - Generate an audio narration from the news script
   - Create a text overlay image for the headline and summary
   - Combine all components into a final video

3. Once completed, the final video file will be available in the project directory, ready for upload to any platform.

---

## 📌 Example Use Case
Imagine you are managing a social media page that posts daily tech news updates.  
Instead of spending hours recording voiceovers, finding stock images, and editing clips, you can run this tool each morning.  
It will automatically pull in the latest news, create narration, fetch relevant visuals, and export ready-to-share videos — all in a matter of minutes.  

Similarly, news publishers can use it to quickly generate breaking news alerts, while bloggers can create visual summaries of their latest articles.

---

## 🔮 Possible Future Enhancements
- Support for multiple languages and regional accents for narration
- Option to add background music tracks
- More sophisticated video templates with animations
- Integration with additional news APIs for broader coverage
- Automatic uploading to YouTube or social media platforms after generation

---

## 📜 License
This project is released under the MIT License.  
See the LICENSE file in the repository for full terms.

---

## 👨‍💻 Author
Developed by Aditya Gaur  
GitHub Profile: [https://github.com/AdityaGaur19](https://github.com/AdityaGaur19)  
Contributions, suggestions, and collaborations are welcome.
