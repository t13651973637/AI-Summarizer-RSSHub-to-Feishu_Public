# RSSHub AI Summarizer for Feishu

An automated n8n workflow that fetches articles from **RSSHub**, generates concise summaries using **AI Agents**, and sends notifications to **Feishu (Lark)**.

## 🚀 Features
- **RSSHub Integration**: Supports any RSSHub feed (News, Papers, etc.).
- **AI-Powered**: Summarizes long articles into structured bullet points.
- **Feishu Bot**: Instant delivery to your team or personal chat.

## 🛠️ Setup
1. Clone this repo.
2. Import `workflow.json` into your **n8n** instance.
3. Configure your **OpenAI/DeepSeek API Key** and **Feishu Webhook URL**.

## 📄 License
MIT

## 📄 Tips
1. Webhook Configuration: To implement this workflow, you must input the Custom Bot Webhook URL from your Feishu (Lark) group chat into the URL field of the HTTP Request node.
2. Model Flexibility: The chat model within the AI Agent node can be customized or replaced according to your preferences.
3. Feed Customization: The URLs in the RSS Read nodes can be updated based on the specific content sources you wish to monitor.
4. Token Management: Ensure the Batch Size in the Loop node is not set too high. Overloading the chat model with too many tokens at once may cause the process to terminate or error out.
