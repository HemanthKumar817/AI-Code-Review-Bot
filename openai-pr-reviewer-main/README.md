# 🤖 AI Code Review Bot

This project uses OpenAI’s powerful language models to review pull requests automatically. It provides intelligent feedback on code quality, design, documentation, and potential bugs — saving developer time and improving code quality.

## 🚀 Features

- 💬 Reviews GitHub Pull Requests using OpenAI's GPT
- 🧠 Highlights issues in logic, readability, or style
- 🔍 Suggests improvements based on best practices
- 🔄 Can be integrated into GitHub Actions or CI/CD pipelines
- 📝 Summarizes PRs in plain English

---

## 🛠️ Tech Stack

- **Python 3.9+**
- [OpenAI API](https://platform.openai.com/)
- [GitHub API](https://docs.github.com/en/rest)
- [LangChain](https://www.langchain.com/) *(optional depending on repo)*
- [dotenv](https://pypi.org/project/python-dotenv/) for managing secrets

---

## 📦 Installation

### 1. Clone the repository

```bash
git clone https://github.com/HemanthKumar817/AI-Code-Review-Bot.git
cd AI-Code-Review-Bot
2. Install dependencies
bash
Copy
Edit
pip install -r requirements.txt
3. Configure API Keys
Create a .env file in the root of the project:

env
Copy
Edit
OPENAI_API_KEY=your_openai_api_key_here
GITHUB_TOKEN=your_github_personal_access_token
⚠️ Never commit your .env file. It's ignored by .gitignore.

🚦 Usage
Depending on your setup, you can use the bot in different ways:

🔧 Manual Review
bash
Copy
Edit
python review_pr.py --repo owner/repo --pr 42
This will fetch the PR diff and run the AI review.

🔄 GitHub Actions (CI/CD)
You can integrate this bot into your GitHub workflow to auto-review PRs and post feedback as comments.

📂 Project Structure
bash
Copy
Edit
AI-Code-Review-Bot/
├── review_pr.py         # Main script to fetch and review PRs
├── github_api.py        # Handles GitHub API interactions
├── openai_api.py        # Interacts with OpenAI
├── .env                 # Secrets (not included in Git)
├── requirements.txt     # Python dependencies
└── README.md            # This file
📌 To-Do / Ideas
 Add support for multiple file diffs

 Fine-tune prompts for security/code smells

 Slack or email notifications

 Automated test coverage suggestions

🙏 Credits
Based on concepts by OpenAI & GitHub community

Inspired by openai-pr-reviewer

📜 License
MIT License. Free to use, modify, and share.

yaml
Copy
Edit

---

Let me know if:
- You want this saved to a file and uploaded directly
- You’d like a version with **badges**, **screenshots**, or **GitHub Action workflow YAML**
- You’re planning to host this as a public GitHub App — I can help with that too!








Ask ChatGPT
