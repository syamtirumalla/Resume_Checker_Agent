# Resume_Checker_Agent

---

## 🧠 AI Instruction Logic

The agent is programmed to follow a specific "Action Required" protocol:
*   **Greetings**: Welcome the user and explain the bot's purpose[cite: 1].
*   **Evaluation**: Request a Google Doc link with clear instructions[cite: 1].
*   **Reporting**: Confirm receipt of links and offer to send the final report via email[cite: 1].

---

## 🛡️ Tech Stack
*   **Logic**: AI-Agent Integration[cite: 1]
*   **Interface**: Telegram API[cite: 1, 2]
*   **Content**: Google Docs API[cite: 4]
*   **Communication**: Gmail API[cite: 3]
*   **Processing**: Regular Expressions (Regex)Here is a comprehensive `README.md` file tailored for your GitHub repository. It organizes the technical components of your **Resume Checker Agent** into a professional structure suitable for a portfolio project.

---

# 🤖 Resume Checker AI Agent

An end-to-end automated pipeline that transforms a **Telegram Bot** into a professional career assistant. This agent extracts resume content from Google Docs, performs an AI-driven evaluation, and delivers detailed reports via Telegram and Gmail.

## 🌟 Overview

The **Resume Checker Agent** is built using a modular workflow architecture. It allows users to submit their resumes via a simple chat interface and receive high-quality feedback based on modern hiring standards.

### 🔄 The Workflow
1.  **Interaction**: User initiates a chat on Telegram[cite: 1].
2.  **Extraction**: The system parses Google Doc links using Regex to retrieve document content[cite: 4].
3.  **Evaluation**: A dedicated **AI Resume Evaluator** analyzes the text[cite: 1].
4.  **Delivery**: Results are pushed to the user via Telegram messages[cite: 2] and a formal Gmail report[cite: 3].

---

## 🛠️ Project Components

This repository contains the following automation blueprints (JSON) that power the agent:

### 1. `Telegram Watch Updates.blueprint .json`
The **Command Center** of the project. This workflow:
*   Connects to the Telegram Webhook to monitor incoming messages[cite: 1].
*   Houses the **AI Agent** logic, which is trained to handle greetings, guide users to provide links, and process resume data[cite: 1].
*   Routes the conversation flow based on user intent (Greeting, Link Submission, or Email Request)[cite: 1].

### 2. `Get Resume Content.blueprint .json`
The **Data Extraction** engine. It performs two critical tasks:
*   **Regex Parsing**: Uses the pattern `/d/(?<docId>[^/]+)/` to identify the unique Google Document ID from a URL[cite: 4].
*   **API Integration**: Communicates with the Google Docs API to fetch the full text body for analysis[cite: 4].

### 3. `Send Message.blueprint.json`
The **Notification** module. 
*   Standardizes the delivery of text updates to the user[cite: 2].
*   Allows the AI to communicate progress and brief summaries back to the Telegram Chat ID[cite: 2].

### 4. `Send Email.blueprint .json`
The **Reporting** module.
*   Triggers after a successful evaluation when the user provides an email address[cite: 3].
*   Sends a structured "Resume Evaluation" email via **Gmail** containing the full AI-generated report[cite: 3].

---

## 🚀 Getting Started

### Prerequisites
*   A **Telegram Bot Token** (from [@BotFather](https://t.me/botfather)).
*   A **Google Cloud Project** with Google Docs and Gmail APIs enabled.
*   An account on an automation platform like **Make.com** to import these blueprints.

### Installation
1.  **Clone the Repo**:
    ```bash
    git clone https://github.com/syamtirumalla/Resume_Checker_Agent.git
    ```
2.  **Import Blueprints**: Upload each `.json` file into your automation environment.
3.  **Configure Connections**:
    *   Update the `__IMTCONN__` and `__IMTHOOK__` fields with your specific API credentials[cite: 1, 2, 3, 4].
4.  **Set Up the AI Agent**: Ensure your LLM agent (e.g., GPT-4 or Gemini) is connected to the `RunAnAIAgent` module in the main flow[cite: 1].

---

## 🧠 AI Instruction Logic

The agent is programmed to follow a specific "Action Required" protocol:
*   **Greetings**: Welcome the user and explain the bot's purpose[cite: 1].
*   **Evaluation**: Request a Google Doc link with clear instructions[cite: 1].
*   **Reporting**: Confirm receipt of links and offer to send the final report via email[cite: 1].

---

## 🛡️ Tech Stack
*   **Logic**: AI-Agent Integration[cite: 1]
*   **Interface**: Telegram API[cite: 1, 2]
*   **Content**: Google Docs API[cite: 4]
*   **Communication**: Gmail API[cite: 3]
*   **Processing**: Regular Expressions (Regex)[cite: 4]

---

### License
This project is open-source and available under the [MIT License](LICENSE).

Here is a comprehensive `README.md` file tailored for your GitHub repository. It organizes the technical components of your **Resume Checker Agent** into a professional structure suitable for a portfolio project.

---

# 🤖 Resume Checker AI Agent

An end-to-end automated pipeline that transforms a **Telegram Bot** into a professional career assistant. This agent extracts resume content from Google Docs, performs an AI-driven evaluation, and delivers detailed reports via Telegram and Gmail.

## 🌟 Overview

The **Resume Checker Agent** is built using a modular workflow architecture. It allows users to submit their resumes via a simple chat interface and receive high-quality feedback based on modern hiring standards.

### 🔄 The Workflow
1.  **Interaction**: User initiates a chat on Telegram[cite: 1].
2.  **Extraction**: The system parses Google Doc links using Regex to retrieve document content[cite: 4].
3.  **Evaluation**: A dedicated **AI Resume Evaluator** analyzes the text[cite: 1].
4.  **Delivery**: Results are pushed to the user via Telegram messages[cite: 2] and a formal Gmail report[cite: 3].

---

## 🛠️ Project Components

This repository contains the following automation blueprints (JSON) that power the agent:

### 1. `Telegram Watch Updates.blueprint .json`
The **Command Center** of the project. This workflow:
*   Connects to the Telegram Webhook to monitor incoming messages[cite: 1].
*   Houses the **AI Agent** logic, which is trained to handle greetings, guide users to provide links, and process resume data[cite: 1].
*   Routes the conversation flow based on user intent (Greeting, Link Submission, or Email Request)[cite: 1].

### 2. `Get Resume Content.blueprint .json`
The **Data Extraction** engine. It performs two critical tasks:
*   **Regex Parsing**: Uses the pattern `/d/(?<docId>[^/]+)/` to identify the unique Google Document ID from a URL[cite: 4].
*   **API Integration**: Communicates with the Google Docs API to fetch the full text body for analysis[cite: 4].

### 3. `Send Message.blueprint.json`
The **Notification** module. 
*   Standardizes the delivery of text updates to the user[cite: 2].
*   Allows the AI to communicate progress and brief summaries back to the Telegram Chat ID[cite: 2].

### 4. `Send Email.blueprint .json`
The **Reporting** module.
*   Triggers after a successful evaluation when the user provides an email address[cite: 3].
*   Sends a structured "Resume Evaluation" email via **Gmail** containing the full AI-generated report[cite: 3].

---

## 🚀 Getting Started

### Prerequisites
*   A **Telegram Bot Token** (from [@BotFather](https://t.me/botfather)).
*   A **Google Cloud Project** with Google Docs and Gmail APIs enabled.
*   An account on an automation platform like **Make.com** to import these blueprints.

### Installation
1.  **Clone the Repo**:
    ```bash
    git clone https://github.com/syamtirumalla/Resume_Checker_Agent.git
    ```
2.  **Import Blueprints**: Upload each `.json` file into your automation environment.
3.  **Configure Connections**:
    *   Update the `__IMTCONN__` and `__IMTHOOK__` fields with your specific API credentials[cite: 1, 2, 3, 4].
4.  **Set Up the AI Agent**: Ensure your LLM agent (e.g., GPT-4 or Gemini) is connected to the `RunAnAIAgent` module in the main flow[cite: 1].

---

## 🧠 AI Instruction Logic

The agent is programmed to follow a specific "Action Required" protocol:
*   **Greetings**: Welcome the user and explain the bot's purpose[cite: 1].
*   **Evaluation**: Request a Google Doc link with clear instructions[cite: 1].
*   **Reporting**: Confirm receipt of links and offer to send the final report via email[cite: 1].

---

## 🛡️ Tech Stack
*   **Logic**: AI-Agent Integration[cite: 1]
*   **Interface**: Telegram API[cite: 1, 2]
*   **Content**: Google Docs API[cite: 4]
*   **Communication**: Gmail API[cite: 3]
*   **Processing**: Regular Expressions (Regex)[cite: 4]

---
