# **Auto Post AI Videos to Social Media with Veo3 and Blotato**

## **Overview**

This **n8n** workflow automates the complete AI video creation and publishing pipeline. It generates a video idea using GPT-4.1, creates a Veo3-compatible prompt, generates a video with Google Veo3 (via Fal API), stores the generated assets in Google Sheets, uploads the final video to Blotato, and publishes it across multiple social media platforms.

---

## **Workflow Steps**

### **Step 1 — Generate Script & Prompt with AI**

- Trigger workflow on schedule.
- Generate a viral video idea using GPT-4.1.
- Generate:
  - Caption
  - Idea
  - Environment
  - Production Status
- Save generated content to Google Sheets.
- Generate a Veo3-compatible cinematic prompt using GPT-4.1.

---

### **Step 2 — Create Video Using Veo3**

- Send the generated prompt to the Veo3 API.
- Wait for video generation.
- Retrieve the final video URL.
- Save the final video URL back to Google Sheets.

---

### **Step 3 — Publish Video to Social Media**
- Read the generated video from Google Sheets.
- Upload the video to Blotato.
- Publish the video to:

- Instagram
- YouTube
- TikTok
- Facebook
- Threads
- Twitter
- LinkedIn
- Bluesky
- Pinterest

- Update the Google Sheet status to **Publish**.

---

## **Services Used**

- OpenAI GPT-4.1
- Google Veo3 (Fal API)
- Blotato API
- Google Sheets

---

## **Social Platforms**

- Instagram
- YouTube
- TikTok
- Facebook
- Threads
- Twitter
- LinkedIn
- Bluesky
- Pinterest

---

## **Required Credentials**
- OpenAI API
- Fal API
- Blotato API
- Google Sheets

---

## **Workflow Flow**

1. Schedule Trigger
2. Generate Video Idea
3. Save Idea to Google Sheets
4. Generate Veo3 Prompt
5. Generate Video with Veo3
6. Wait for Processing
7. Retrieve Final Video URL
8. Save Video URL to Google Sheets
9. Upload Video to Blotato
10. Publish to Social Media Platforms
11. Update Google Sheets Status

---

## **Google Sheets Fields**

- id
- idea
- caption
- production
- environment_prompt
- final_output
- PROMPT
- DESCRIPTION
- URL VIDEO
- Titre
- STATUS
- row_number

---

## **APIs Used**

- OpenAI GPT-4.1
- Fal AI Veo3 API
- Blotato Media API
- Blotato Posts API
- Google Sheets API

---

## **Features**

- AI-generated viral video ideas
- Automatic caption generation
- Veo3 prompt generation
- AI video generation
- Google Sheets integration
- Automatic video upload
- Multi-platform social media publishing
- Daily scheduled execution
