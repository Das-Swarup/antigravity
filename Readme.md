
# Getting started with Google Antigravity  
## Build with Gemini CLI + Antigravity IDE + Cloud Run

Welcome to the hands-on workshop!

In this session, you will:

- ✅ Create a Google Cloud Project (using UI)
- ✅ Enable required services
- ✅ Generate a Gemini API Key
- ✅ Use Gemini CLI to generate your portfolio
- ✅ Open the project manually in Antigravity IDE
- ✅ Deploy to Cloud Run from Antigravity
- ✅ Get a live public URL 🎉

---

# Prerequisites

Make sure you have:

- A Google Account
- A Laptop/Desktop (Windows / macOS / Linux)
- Google Chrome Browser
- Stable Internet
- Node.js (v6 or above)

Check Node installation:

```bash
node -v
````

If not installed:
[https://nodejs.org](https://nodejs.org)

And follow the steps mentioned as per your OS

---

# STEP 1 – Create Google Cloud Project (Using UI)

1. Open:
   [https://console.cloud.google.com](https://console.cloud.google.com)

2. Click the **Project Dropdown (Top Left)**

3. Click **New Project**

4. Enter:

   * Project Name: `my-portfolio`
   * Location: Leave default (if personal Gmail)

5. Click **Create**

6. Make sure your new project is selected.

---

# STEP 2 – Enable Required APIs (Using UI)

Go to:
[https://console.cloud.google.com/apis/library](https://console.cloud.google.com/apis/library)

Enable the following APIs:

### ✅ Cloud Run API

Search → [`Cloud Run API`](https://console.cloud.google.com/marketplace/product/google/run.googleapis.com?q=search&referrer=search&project=upheld-magpie-488012-a3) → Click → Enable

### ✅ Cloud Build API

Search → [`Cloud Build API`](https://console.cloud.google.com/marketplace/product/google/cloudbuild.googleapis.com?referrer=search&project=upheld-magpie-488012-a3&returnUrl=%2Fcloud-build%2Fbuilds%3Freferrer%3Dsearch%26project%3Dupheld-magpie-488012-a3) → Enable

### ✅ Artifact Registry API

Search → [`Artifact Registry API`](https://console.cloud.google.com/marketplace/product/google/artifactregistry.googleapis.com?q=search&referrer=search&project=upheld-magpie-488012-a3) → Enable

### ✅ Generative Language API (Gemini)

Search → [`Gemini API`](https://console.cloud.google.com/marketplace/product/google/generativelanguage.googleapis.com?q=search&referrer=search&project=upheld-magpie-488012-a3) → Enable

---

# STEP 3 – Generate Gemini API Key

1. Go to:
   [https://aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)

2. Click **Create API Key**

3. Copy the key

Now set it in your system:

### macOS / Linux

```bash
export GEMINI_API_KEY="PASTE_YOUR_KEY"
```

### Windows (PowerShell)

```powershell
setx GEMINI_API_KEY "PASTE_YOUR_KEY"
```

Restart your terminal after this.


# STEP 4 – Generate Your Project root folder

Create a new folder:

```bash
mkdir my-projects
cd my-projects
```

---

# STEP 5 – Open Project in Antigravity IDE


1. Open **Google Antigravity IDE**.

2. Click **Open Project** or **Open Folder**

3. Choose: `my-projects`

4. Wait for Antigravity to load the project folder.

5. Open the antigravity agent manager using `Ctrl+E`

6. Select the project folder in agent manager from left sidebar

7. Paste your choice of prompt from the set of prompts from the prompt.md file.

---

# STEP 6 – Preview Your Project

Inside Antigravity:

* Check the files being created
* Review and select `Run` when it asks and wait till Antigravity creates all the files
* Open `[localhost:3000](localhost:3000)
* Verify the project is  loaded

If something is broken, we have to fix it before deploying.

---

# STEP 7 – Deploy to Cloud Run from Antigravity

Inside Antigravity:

1. Go to **Editor** or press `Ctrl+E` from agent manager.
2. Now open the agent sidebar using `Ctrl+L`. This should open a sidebar to the right side.
3. Now from the top right there will be **3 dots**, click on that and select **MCP Servers** from dropdown.
4. Search for `Cloud Run` in the search textbox on the MCP Store. Hover on the Cloud Run MCP server, and click on the Install button that appears to the right.
5. Once installed, click on the Back to Agent button at the top of the Agent Manager panel.
6. On the Agent Manager panel, we will now prompt to deploy this folder as Cloud Run service on the Google Cloud project as follows:

   ```
   Deploy this folder as Cloud Run service in the project <yout-project-id> in asia-south1 region.
   ```

Wait 2–5 minutes.

You will receive a URL like:

```
https://your-project-name-xxxxx.run.app
```

🎉 This is your live project!

---

# STEP 8 – Test Your Live Website

Open your deployed URL and verify:

* Mobile responsiveness
* Usability
* Scope for improvements
* Clean layout

Share your URL with classmates 

---

# Workshop Flow Summary

1. Create Cloud Project (UI)
2. Enable APIs (UI)
3. Generate Gemini API Key
4. Generate Portfolio Code
5. Open Folder in Antigravity IDE
6. Deploy to Cloud Run
7. Get Live URL

---

# Expected Outcome

By the end of this workshop, you will have:

* ✅ A project to showcase in your resume
* ✅ Hosted on Google Cloud Run
* ✅ A public live URL
* ✅ Real cloud deployment experience
* ✅ Hands-on AI-assisted development experience

---

# 🏁 Final Note

Keep improving it even after the workshop 
