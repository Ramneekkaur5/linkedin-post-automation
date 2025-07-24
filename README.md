# 🚀 LinkedIn AI Image Post Generator (n8n Workflow)

This project automates the creation and posting of AI-generated LinkedIn posts using:
- **n8n** for workflow automation
- **Groq/OpenAI** for generating content
- **OpenAI Image API** for visuals
- **LinkedIn API** to auto-publish posts

---

## 🛠️ Features

- Generate captions using AI Agent (Groq/OpenAI)
- Generate image via OpenAI DALL·E API
- Combine both (merge node)
- Post to LinkedIn automatically

---

## 🧩 Workflow Overview

<img width="1186" height="388" alt="image" src="https://github.com/user-attachments/assets/e3898268-06f9-4461-8abd-b8003b202b56" />


---

## 📦 Installation

1. **Clone or import workflow**

   - Clone this repo or download `linkedin_post_creator.json`.
   - In n8n, go to **Workflows → Import**, and upload the JSON file.

2. **Install and start n8n** (if not already)

   ```bash
   npm install n8n -g
   n8n start
   ```
---

## ⚙️ Configuration

1. **Set up credentials**

   - In n8n, add a **GeminiChatBot** credential using your `GEMINI_API_KEY`.
   - Add a **LinkedIn OAuth2** credential for publishing (Client ID/Secret).

2. **Form URL**

   - Note the webhook URL displayed on the **On form submission** node; embed it in your front-end form or share it with users.

3. **Enable Workflow**

   - Toggle the workflow from **inactive** to **active** in n8n.
---

## 🚀 Usage & Workflow
This project automates the process of creating and posting AI-generated content on LinkedIn using n8n workflows.

🔁 Workflow Steps:
📝 Form Submission – User submits input via a form.

🧠 Gemini Model – Generates captions/content from input.

🛠️ Edit Fields – Cleans and formats the content.

🖼️ Image Generation – Creates a visual using the content via image API.

🧮 Code Node – Custom logic for formatting or combining data.

🔗 Merge – Combines text and image for the final post.

📤 LinkedIn Post – Publishes the content with image and caption.

---
## 📄 License

Distributed under the MIT License. See [LICENSE](LICENSE) for details.

