# End to End AI Agent Customer Sentiment Automation
### Built with n8n + Google Gemini API key


##  Project Overview
This project is an end-to-end AI-driven workflow built in **n8n** that automates the entire customer feedback loop. By leveraging **Google Gemini API**, the system interprets human emotion in text, categorizes it, and responds instantly—bridging the gap between data collection and customer engagement.

##  Key Objectives
* **Automate** customer feedback collection from forms.
* **Analyze** sentiment using advanced Large Language Models (LLMs).
* **Trigger** dynamic, context-aware email responses via Gmail.
* **Log** structured data into Google Sheets for long-term Analytics.
* **Showcase** a production-ready AI-integrated automation pipeline.

---

## AI Workflow Logic

The workflow follows a 5-step intelligent sequence:

### 1. Form Trigger
The process begins when a customer submits a feedback form containing:
* Name, Email, and Phone Number.
* **Feedback Text** (The raw data for analysis).

### 2. AI Sentiment Analysis
The feedback text is processed by a **Google Gemini AI Agent**, which performs classification:

| AI Output | Meaning |
| :--- | :--- |
| **Good** | Positive Sentiment |
| **Neutral** | Neutral Sentiment |
| **Negative** | Negative or bad Sentiment |

### 3. Merge & Classification
Using an n8n **Switch Node**, the workflow routes the data based on the AI's verdict to ensure the correct follow-up action is taken.

### 4. Automated Email Response
Personalized emails are dispatched via the **Gmail Node**:
* **Positive:** Appreciation and brand loyalty reinforcement.
* **Neutral:** Acknowledgement and request for specific improvement ideas.
* **Negative:** Immediate apology and assurance of manual escalation.

### 5. Data Logging
All interactions are logged in **Google Sheets** across dedicated tabs (Positive/Neutral/Negative) for easy reporting. Fields tracked include:
`Name` | `Email` | `Phone` | `Feedback` | `Message ID` | `Status`

---

## Tech Stack

| Technology | Purpose |
| :--- | :--- |
| **n8n Automation** | Workflow orchestration and logic routing |
| **Google Gemini AI** | NLP and Sentiment Analysis |
| **Gmail API** | Automated personalized communication |
| **Google Sheets API** | Structured data storage and logging |
| **No-code / Low-code** | Rapid deployment and scalability |

---

## Key Features
*  **Real-time Sentiment Classification:** No manual reading required.
*  **Dynamic Routing:** Intelligent branching using Switch logic.
*  **Automated Personalization:** Responses tailored to the user's mood.
*  **Scalable Design:** Can be adapted for CRMs like Salesforce or HubSpot.
### Setup Notes
* n8n Version: Built on n8n Cloud.
* API Keys Required: Google Cloud Console (Gemini API).

Adaptability: This logic can easily be ported to Slack, Discord, or WhatsApp Business for different notification styles.

Author
Saptarshi Bandyopadhyay Data Analyst | AI and Automation Enthusiast
---
