# 🛍️ AI Shopping Advisor Agent

An AI-powered Shopping Advisor Agent built using **n8n**, **Google Gemini**, and the **DummyJSON Products API**.

This project helps users find suitable products based on their natural-language requirements such as product category, maximum price, minimum rating, discount, and brand. The AI analyzes the available products and provides a **Best Recommendation** along with **two alternative products**.

The final recommendation can also be formatted as an **HTML email** and sent directly to the user's Gmail account.

---

## 🚀 Features

- 🤖 AI-powered shopping recommendations
- 💬 Accepts natural-language shopping queries
- 🔍 Extracts user requirements automatically
- 🛒 Fetches product data using DummyJSON API
- 🧩 Dynamically filters products based on user requirements
- 💰 Supports maximum price filtering
- ⭐ Supports minimum rating filtering
- 🏷️ Supports product category filtering
- 📊 Analyzes price, rating, discount, stock, and brand
- 🏆 Provides the Best Recommendation
- 🥈 Provides Alternative Recommendation 1
- 🥉 Provides Alternative Recommendation 2
- 📧 Sends recommendations through Gmail
- 🎨 Supports HTML and CSS formatted email output

---

## 🧠 How the Project Works

The workflow follows these steps:

```text
User Shopping Query
        ↓
AI Agent
        ↓
Extract Shopping Requirements
        ↓
HTTP Request
        ↓
DummyJSON Products API
        ↓
Split Out Products
        ↓
Filter Products
        ↓
Aggregate Matching Products
        ↓
AI Shopping Advisor Agent
        ↓
Generate Recommendations
        ↓
JavaScript HTML Formatter
        ↓
Gmail
        ↓
User Receives Recommendation Email

---

## 📷 Screenshots

Example screenshot (place your image at `screenshots/workflow-screenshot.svg`):

![Workflow Screenshot](screenshots/workflow-screenshot.svg)

How to add your screenshot:

1. Save or move your image file into the `screenshots/` folder with the name `workflow-screenshot.png`.
2. Commit the change:

```bash
git add screenshots/workflow-screenshot.png
git commit -m "Add workflow screenshot"
git push
```

If you prefer PowerShell on Windows, use:

```powershell
# from the directory where your downloaded image is located
Move-Item -Path .\YourImageFile.png -Destination .\screenshots\workflow-screenshot.png
git add screenshots\workflow-screenshot.png
git commit -m "Add workflow screenshot"
git push
```