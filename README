# Testing the Gemini Code Review Agent

This guide provides step-by-step instructions on how to set up a local test environment and run the `code_review_agent.py` script to review code changes.

---

## 1. Environment Setup

### Prerequisites
- Python 3.10+
- Git

### Configure Your API Key
The agent requires a **Gemini API key** to function.

1. Obtain your API key from [Google AI Studio](https://aistudio.google.com/).
2. Set it as an environment variable.  

**macOS/Linux:**
```bash
export GEMINI_API_KEY='YOUR_API_KEY_HERE'
```

**Windows (Command Prompt):**
```cmd
set GEMINI_API_KEY=YOUR_API_KEY_HERE
```

**Windows (PowerShell):**
```powershell
$Env:GEMINI_API_KEY="YOUR_API_KEY_HERE"
```

> **Note:** You must run this command in the same terminal session where you will execute the Python script.

---

## 2. Clone the Git Test Project

```bash
git clone https://github.com/xkaple00/test_task_part_2.git
cd test_task_part_2
```

### Install Dependencies
Using Conda:
```bash
conda create -n test_task python=3.10
conda activate test_task
pip install -r requirements.txt
```

---

## 3. Run the Code Review Agent

Make sure your `code_review_agent.py` script is in the **parent directory** of `test_task_part_2`.

Run:
```bash
python code_review_agent.py ./test_task_part_2 feature/add-subtraction
```

---

## Expected Outcome

You should see progress messages like:

```
Starting code review for branch 'feature/add-subtraction' in repository './test_task_part_2'...
Successfully generated diff. Sending to Gemini for review...
Review complete. Comments saved to 'review_comments.txt'.
```

A new file named **`review_comments.txt`** will be created in the same directory.  
This file will contain the AI's detailed code review.  

---
