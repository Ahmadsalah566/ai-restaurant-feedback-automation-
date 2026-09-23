# 🍽️ AI Restaurant Feedback & Automated Notification System

An end-to-end AI automation workflow built with **n8n** that collects customer feedback and reviews for restaurants, performs sentiment analysis using **Google Gemini LLM**, stores structured logs in **Google Sheets**, and **automatically sends instant email notifications to the restaurant team and customers**.

---

## 🌟 Key Capabilities

- **Customer Feedback Collection:** Captures ratings, reviews, and customer details via a clean web form.
- **AI Sentiment & Priority Analysis:** Evaluates customer satisfaction, categorizes issues, and scores the overall experience using Gemini LLM.
- **Automated Instant Notifications:** Automatically dispatches email responses to acknowledge receipt and notify management.
- **Centralized Data Storage:** Automatically appends every review into an organized Google Sheet dashboard.

---

## 🏗️ Workflow Architecture

1. **n8n Form Trigger:** Receives customer feedback and star ratings.
2. **JavaScript Processing Node:** Validates inputs, calculates message length, and structures raw data.
3. **LangChain + Gemini LLM Chain:** Analyzes feedback sentiment, assigns priority levels, and suggests actionable resolution steps.
4. **Structured Output Parser:** Formats AI findings into a standardized JSON Schema.
5. **Google Sheets Integration:** Logs all feedback details and AI scores into the database.
6. **Gmail Automated Dispatch:** Automatically sends custom email notifications.

---

## 🛠️ Tech Stack

- **Automation Engine:** n8n
- **AI Engine:** Google Gemini API (`lmChatGoogleGemini`)
- **AI Framework:** LangChain Nodes (LLM Chain + Structured Parser)
- **Database:** Google Sheets
- **Communication:** Gmail API

---

## 🚀 Getting Started

1. Download the `restaurant-feedback-workflowN8N.json` file from this repository.
2. Import it into your **n8n** workflow canvas.
3. Set up your **Google Gemini API**, **Google Sheets**, and **Gmail** credentials.
4. Activate the workflow and start receiving customer reviews!
