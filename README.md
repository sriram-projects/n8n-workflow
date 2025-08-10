# WhatsApp-Driven Google Drive Assistant (n8n Workflow)

This project is part of an internship task to create an **n8n workflow** that listens to WhatsApp messages and performs **Google Drive actions** such as listing files, summarising, and (optionally) deleting/moving files.

## 🚀 Features
- **LIST** – Get a list of files in a Google Drive folder  
- **SUMMARY** – Summarise PDF/DOCX/TXT files in the folder using OpenAI GPT-4o  
- **DELETE** – (Planned) Delete files from Google Drive  
- **WhatsApp Integration** – Using Twilio Sandbox for WhatsApp to send/receive commands  
- **Google Drive API** – OAuth2 authentication for accessing files  
- **Audit Logging** – Store actions for tracking and safety

## 📌 Prerequisites
1. **n8n** installed locally or hosted (e.g., Render, Railway, Docker)  
2. **Google Drive API** enabled in Google Cloud Console  
3. **Twilio Sandbox for WhatsApp** account  
4. **OpenAI API key** (for summarisation)  
5. Node.js and npm (if running locally)

---
## 🛠 Setup Instructions

### 1. Clone the Repository

git clone https://github.com/sriram-projects/n8n-workflow.git
cd n8n-workflow


## Import Workflow into n8n

1. Open n8n
2. Click Import from file
3. Select workflow.json from this repository.
4. Configure the credentials for:

Google Drive API

Twilio WhatsApp

OpenAI API


## Usage

Send commands to your WhatsApp-connected Twilio number:

LIST /FolderName
SUMMARY /FolderName
DELETE /FolderName/filename.pdf

## 📂 Project Structure

📦 project-folder
 ┣ 📜 workflow.json         # n8n workflow file
 ┣ 📜 README.md             # Documentation
 ┣ 📜 env-sample            # Environment variable template
 ┗ 📜 helper-scripts/       # (Optional) Any extra code

## 🎥 Demo Video

Click here to watch the demo : https://www.veed.io/view/17d1b8cd-1b55-4a26-a60d-e160b413e184?panel=share

##🧑‍💻 Author

Sriram A.

Student, BE CSE

GitHub: your-github-profile

##⚠️ Notes

The current DELETE function is restricted due to Google Drive API permission scope.

Ensure to enable https://www.googleapis.com/auth/drive for full file access.
