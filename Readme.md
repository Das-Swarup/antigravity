
# Getting started with Google Antigravity  
## Build and Deploy with Antigravity IDE + Cloud Run

Welcome to the hands-on workshop!

In this session, you will:

- ✅ Create a Google Cloud Project
- ✅ Install gcloud CLI
- ✅ Enable required services
- ✅ Generate a Gemini API Key
- ✅ Use Gemini CLI to generate your portfolio
- ✅ Open the project manually in Antigravity IDE
- ✅ Deploy to Cloud Run from Antigravity
- ✅ Get a live public URL for your resume 🎉

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

Check gcloud CLI installation:

```bash
gcloud help
````
If the previous command shows `command not found`:
* Add Google Cloud SDK repo
  ```bash
  sudo apt update
  ```
  ```bash
  sudo apt install apt-transport-https ca-certificates gnupg curl
  ```
  ```bash
  curl -fsSL https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo gpg --dearmor -o /usr/share/keyrings/cloud.google.gpg
  ```
  ```bash
  echo "deb [signed-by=/usr/share/keyrings/cloud.google.gpg] https://packages.cloud.google.com/apt cloud-sdk main" | sudo tee /etc/apt/sources.list.d/google-cloud-sdk.list
  ```
* Install gcloud CLI
   ```bash
   sudo apt update
   ```
   ```bash
   sudo apt install google-cloud-cli
   ```
* Verify Installation
  ```bash
  gcloud --version
  ```
* Initialize
  ```bash
  gcloud init
  ```

---

# STEP 1 – Create Google Cloud Project

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

Note: Some APIs might already be enabled and will show **Manage** instead 'Enable'.

Go to:
[https://console.cloud.google.com/apis/library](https://console.cloud.google.com/apis/library)

Enable the following APIs:

### ✅ Cloud Run API

Search → [`Cloud Run API`](https://console.cloud.google.com/marketplace/product/google/run.googleapis.com?q=search&referrer=search&project=upheld-magpie-488012-a3) → Click → Enable

### ✅ Cloud Build API

Search → [`Cloud Build API`](https://console.cloud.google.com/marketplace/product/google/cloudbuild.googleapis.com?referrer=search&project=upheld-magpie-488012-a3&returnUrl=%2Fcloud-build%2Fbuilds%3Freferrer%3Dsearch%26project%3Dupheld-magpie-488012-a3) → Click → Enable

### ✅ Artifact Registry API

Search → [`Artifact Registry API`](https://console.cloud.google.com/marketplace/product/google/artifactregistry.googleapis.com?q=search&referrer=search&project=upheld-magpie-488012-a3) → Click → Enable

### ✅ Generative Language API (Gemini)

Search → [`Gemini API`](https://console.cloud.google.com/marketplace/product/google/generativelanguage.googleapis.com?q=search&referrer=search&project=upheld-magpie-488012-a3) → Click → Enable

---

# STEP 3 – Generate Gemini API Key (Optional)

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

Open Terminal and run-

```bash
mkdir my-projects
cd my-projects
```

---

# STEP 5 – Open Project in Antigravity IDE


1. Open **Google Antigravity IDE**.

2. Click **Open Project** or **Open Folder** from **Files**

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
  
* Antigravity should run your project by default but if it does not then give command
  ```
  run the project
  ```

* Open `[localhost:3000](localhost:3000) if not opened automatically by Antigravity
  
* Verify the project is loaded and usable

If something is broken, we have to fix it before deploying.

---

# STEP 7 – Deploy to Cloud Run from Antigravity

Inside Antigravity:

1. Go to **Editor** or press `Ctrl+E` from agent manager.
   
3. Now open the agent sidebar using `Ctrl+L`. This should open a sidebar to the right side.
   
5. Now from the top right there will be **3 dots**, click on that and select **MCP Servers** from dropdown.
   
7. Search for `Cloud Run` in the search textbox on the MCP Store. Hover on the Cloud Run MCP server, and click on the Install button that appears to the right.
   
9. Once installed, click on the Back to Agent button at the top of the Agent Manager panel.
    
11. On the Agent Manager panel, we will now prompt to deploy this folder as Cloud Run service on the Google Cloud project as follows:

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
