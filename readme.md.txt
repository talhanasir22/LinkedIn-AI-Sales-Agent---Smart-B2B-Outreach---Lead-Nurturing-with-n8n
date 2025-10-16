# 🚀 LinkedIn AI Sales Agent – Smart B2B Outreach & Lead Nurturing with n8n

This fully automated workflow builds, optimizes, and publishes LinkedIn posts with AI — completely hands-free.
Developed in **n8n**, it integrates **OpenAI**, **Google Sheets**, and intelligent **web scraping** to turn a single keyword into engaging LinkedIn content complete with AI-generated visuals.

---

## ✅ How It Works – Step by Step

### 1. 💬 Keyword Input via Chat

Start the workflow by submitting a keyword (e.g., “AI Agent”) through chat.

### 2. 🔍 Keyword Research

An HTTP request retrieves around 10 trending search terms related to your input.
These keywords form the basis for multiple content variations.

### 3. 🔁 Content Generation Loop

For each of the 10 keywords, the workflow:

* 📝 Writes a LinkedIn post description
* 🧠 Generates a catchy title
* 🎨 Designs an AI-friendly image prompt

All generated outputs are automatically saved in **Google Sheets** for later use or review.

---

## 🧠 Intelligent Content Selection

After looping through all keywords:

* An AI agent scans the web for trending insights
* Chooses the top-performing keyword and post combination
* Runs validation using a **Think node** to ensure quality and relevance

---

## 🖼️ AI Image Creation

The selected prompt is used to:

* Produce a suitable image via an AI model
* Format and optimize it for LinkedIn
* Retrieve the image URL
* Conduct quality checks for resolution, size, and text clarity

---

## 🧪 Quality Assurance Before Publishing

Before going live:

* The workflow verifies image layout and quality
* Ensures content meets professional publishing standards

---

## 📢 Automated LinkedIn Publishing

If all validations pass:

* The post title and description are combined
* The content is automatically published to LinkedIn via a **POST API call**

---

## 📊 Data Tracking & Storage

Post-publication, the system:

* Saves the keyword, post content, and image URL to **Google Sheets**
* Prevents duplicate posts
* Keeps track of unused content for future scheduling

---

## 🧰 Tools Used

* **n8n** – Workflow automation
* **OpenAI** – Text and image generation
* **Google Sheets** – Content logging and management
* **LinkedIn API** – Automated publishing
* *(Optional)* Keyword APIs – e.g., Google Suggest, SERP, Keywords Everywhere

---

## 🔧 Customizable For

* Cross-platform posting (Instagram, X, Facebook)
* Email newsletter automation
* Brand-specific visual customization

---

## 🧠 Ideal For

* Freelancers and creators automating content production
* Agencies managing large-scale post creation
* Marketers seeking consistent, daily engagement
