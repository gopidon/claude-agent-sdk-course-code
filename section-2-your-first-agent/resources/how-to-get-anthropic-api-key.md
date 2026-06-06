# How to Get Your Anthropic API Key

**Build Production AI Agents with the Claude Agent SDK**
Section 2 · Lecture 2.1 Resource

Before you can run any notebook in this course, you need an Anthropic API key.
This guide walks you through every click — from opening your browser to pasting
the key into Colab Secrets.

> ⚠️ **Keep your API key private.** Treat it like a password. Never paste it
> directly into a notebook cell or share it in a screenshot.

---

## Part 1 — Create an Anthropic Account

> Skip to Part 2 if you already have an account.

**Step 1 — Open your browser and go to the Anthropic Console**
Navigate to: https://platform.claude.com/

**Step 2 — Click "Sign up"**
You will see this button in the top-right corner of the page.

**Step 3 — Enter your email address and choose a password**
Or use the "Continue with Google" option to sign up with your Google account —
either works.

**Step 4 — Check your inbox for a verification email**
Click the link in that email to confirm your address. The email comes from
Anthropic and usually arrives within a minute.

**Step 5 — Complete any onboarding prompts**
Anthropic may ask a few questions about your use case. Answer them and continue.

---

## Part 2 — Generate an API Key

**Step 1 — Log in to the Anthropic Console**
Go to https://platform.claude.com/ and sign in if you are not already.

**Step 2 — Click your profile or organisation name in the top-left**
A navigation sidebar will appear on the left side of the screen.

**Step 3 — Click "API Keys" in the left sidebar**
This opens the API key management page. You may see a list of existing keys if
your organisation already has some.

**Step 4 — Click "Create Key"**
A dialog box will appear asking you to name your key.

**Step 5 — Give your key a name**
Use something descriptive like "Udemy Course" or "Claude Agent SDK Learning"
so you can identify it later.

**Step 6 — Click "Create Key" to confirm**
Anthropic will generate your key and display it on screen.

> ⚠️ **IMPORTANT: Copy the key right now.** Anthropic will only show you the
> full key once. After you close this dialog, you cannot retrieve the value
> again — only delete it and create a new one.

**Step 7 — Copy the key**
Click the copy icon next to the key or select the text and copy it manually.
Paste it somewhere temporary (like a text editor) until you add it to Colab
Secrets in the next part.

**Step 8 — Click "Done" or close the dialog**
The key will now appear in your list, but only the first few characters will be
visible — the rest is hidden for security.

---

## Part 3 — Add the Key to Colab Secrets

Colab Secrets is the secure, built-in way to store your API key in Google Colab.
The key is stored against your Google account and never saved inside the notebook
file.

**Step 1 — Open the Lecture 2.1 notebook in Google Colab**
Use the GitHub link in the course resources section to open the notebook. It will
open directly in Colab.

**Step 2 — Find the key icon in the left sidebar**
Look for a small padlock or key icon on the left-hand panel inside Colab. It is
usually the fourth or fifth icon from the top.

**Step 3 — Click the key icon to open the Secrets panel**
A panel slides out from the left showing your stored secrets (it may be empty
the first time).

**Step 4 — Click "+ Add new secret"**
A form appears with two fields: Name and Value.

**Step 5 — Set the Name field to exactly `ANTHROPIC_API_KEY`**
The name must be exact — capital letters, underscores, no spaces. This is the
name the SDK looks for automatically.

**Step 6 — Paste your API key into the Value field**
This is the key you copied from the Anthropic Console in Part 2. Do not add any
extra spaces or line breaks.

**Step 7 — Toggle "Notebook access" to ON**
This is essential. Without it, the code cell in the notebook cannot read the
secret. The toggle must be blue/enabled.

**Step 8 — Close the Secrets panel**
Click elsewhere or press the X. Your secret is now saved.

---

## Part 4 — Verify It Works

**Step 1 — Run Cell 4 in the notebook**
This cell reads the secret and loads it into the environment. If you see a
pop-up asking for permission, click Allow.

**Step 2 — Run Cell 5 in the notebook**
This cell imports the SDK and checks that the key is present. You should see:

```
SDK installed successfully!
API key set: True
```

> ⚠️ If you see `API key set: False` — go back to Part 3 and make sure the
> **Notebook access** toggle is ON, then re-run Cells 4 and 5.

---

## Troubleshooting

**"I can't find the Secrets panel"**
Look for the key/padlock icon in the very left edge of the Colab interface.
If you don't see it, try refreshing the page.

**"I closed the key dialog before copying"**
You will need to generate a new key. Go back to Part 2 Step 4, create a new
key, and copy it immediately.

**"I get an authentication error when running agent code"**
Make sure the secret name is exactly `ANTHROPIC_API_KEY` with no typos, and
that you re-run the key-loading cell after any session restart.

**"My Colab session restarted and now the key is gone"**
The secret itself is safely stored. You just need to re-run Cell 4 (the
loading cell) to put it back into `os.environ` for the new session.

---

*Anthropic Console · [platform.claude.com](https://platform.claude.com/) ·
Build Production AI Agents with the Claude Agent SDK*
