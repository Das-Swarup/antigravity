````markdown
# 🚀 Getting started with Google Antigravity  
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
- Node.js (v18 or above)

Check Node installation:

```bash
node -v
````

If not installed or version is less than 18:
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

Search → `Cloud Run API` → Click → Enable

### ✅ Cloud Build API

Search → `Cloud Build API` → Enable

### ✅ Artifact Registry API

Search → `Artifact Registry API` → Enable

### ✅ Generative Language API (Gemini)

Search → `Generative Language API` → Enable

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

---

# STEP 4 – Install Gemini CLI

Install globally:

```bash
npm install -g @google/gemini-cli
```

Verify:

```bash
gemini --version
```

---

# STEP 5 – Generate Your Portfolio Project

Create a new folder:

```bash
mkdir my-portfolio
cd my-portfolio
```

Start Gemini CLI:

```bash
gemini
```

Inside Gemini CLI:

👉 Paste the portfolio prompt provided during the workshop.

Wait until all files are generated.

You should now see project files inside your `my-portfolio` folder.

---

# STEP 6 – Open Project in Antigravity IDE (Manual Method)

⚠️ We are NOT using Antigravity CLI.

1. Open **Google Antigravity IDE** in your browser.

2. Click **Open Project** or **Open Folder**

3. Choose:

   ```
   my-portfolio
   ```

4. Wait for Antigravity to load the project.

You should now see:

* File structure
* Preview option
* Deploy button

---

# STEP 7 – Preview Your Project

Inside Antigravity:

* Click **Preview**
* Check layout
* Verify sections load correctly

If something is broken, fix it before deploying.

---

# STEP 8 – Deploy to Cloud Run from Antigravity

Inside Antigravity:

1. Click **Deploy**
2. Select:

   ```
   Cloud Run
   ```
3. Choose your Google Cloud Project
4. Select region (Recommended: `asia-south1`)
5. Allow unauthenticated access
6. Click **Deploy**

Wait 2–5 minutes.

You will receive a URL like:

```
https://your-project-name-xxxxx.run.app
```

🎉 This is your live portfolio website!

---

# STEP 9 – Test Your Live Website

Open your deployed URL and verify:

* Mobile responsiveness
* Project links
* Contact section
* Clean layout

Share your URL with classmates 

---

# Workshop Flow Summary

1. Create Cloud Project (UI)
2. Enable APIs (UI)
3. Generate Gemini API Key
4. Install Gemini CLI
5. Generate Portfolio Code
6. Open Folder in Antigravity IDE
7. Deploy to Cloud Run
8. Get Live URL

---

# Expected Outcome

By the end of this workshop, you will have:

* ✅ A professional portfolio website
* ✅ Hosted on Google Cloud Run
* ✅ A public live URL
* ✅ Real cloud deployment experience
* ✅ Hands-on AI-assisted development experience

---

# 🏁 Final Note

Keep improving it even after the workshop 
