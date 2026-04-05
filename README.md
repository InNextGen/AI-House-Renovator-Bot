# 🏡 AI House Renovator: Automated Interior Design Bot

An advanced, fully automated AI workflow that acts as a virtual interior designer. Users can simply send a photo of an empty or old room via Telegram, and the AI will analyze the space, generate stunning renovated concepts, and deliver a smooth "Before & After" transition video.

## 📸 Workflow Architecture
<img width="1132" height="547" alt="Screenshot 2569-04-05 at 23 48 22" src="https://github.com/user-attachments/assets/018fb45e-aef5-44a8-aa3c-a9e8ea4c919f" />

## ✨ Key Features
- **Seamless Telegram Interface:** Users interact with the system entirely through a Telegram Bot. Just snap a photo of a room and hit send.
- **Intelligent Vision Analysis:** Utilizes **OpenAI Agents & Vision** to analyze the uploaded image, understanding the room's layout, lighting, and structure.
- **Generative Remodeling:** Automatically drafts precise prompts and calls Image Generation APIs to create highly realistic, renovated versions of the space.
- **Dynamic Video Transitions:** Incorporates Video AI APIs to stitch the original and generated images together, creating an engaging, smooth transition video showing the transformation.
- **Automated Tracking:** Logs all requests, generated image links (via ImgBB), and process statuses into **Google Sheets** for easy monitoring and database management.

## 🛠️ Tech Stack & Integrations
- **Automation Engine:** n8n
- **User Interface:** Telegram Bot API
- **AI Brain:** OpenAI (GPT-4o, AI Agents, Structured Output Parsers)
- **Generative Media APIs:** Image Generation & Video Stitching Tools
- **Data Storage:** Google Sheets, ImgBB

## 🚀 How It Works (The Pipeline)
1. **Input:** The Telegram trigger receives an image file from the user.
2. **Analysis:** An AI Agent analyzes the image and conceptualizes a renovation design.
3. **Image Generation:** The workflow sends an API request to generate the renovated room.
4. **Video Processing:** A looping mechanism waits for the image generation to complete, then triggers a video AI tool to create a smooth transition from the old room to the new one.
5. **Delivery:** The finalized images and the transition video are sent directly back to the user's Telegram chat.

---
*Developed by Non Poramat | Showcasing the power of AI Agents, API Integrations, and Workflow Automation*
