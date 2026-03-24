<header>

<!--
  <<< Author notes: Course header >>>
  Read <https://skills.github.com/quickstart> for more information about how to build courses using this template.
  Include a 1280×640 image, course name in sentence case, and a concise description in emphasis.
  In your repository settings: enable template repository, add your 1280×640 social image, auto delete head branches.
  Next to "About", add description & tags; disable releases, packages, & environments.
  Add your open source license, GitHub uses the MIT license.
-->

# Code with GitHub Copilot

_GitHub Copilot can help you code by offering autocomplete-style suggestions right in VS Code and Codespaces._

</header>

<!--
  <<< Author notes: Step 1 >>>
  Choose 3-5 steps for your course.
  The first step is always the hardest, so pick something easy!
  Link to docs.github.com for further explanations.
  Encourage users to open new tabs for steps!
-->

## Step 1: Leverage Codespaces with VS Code for Copilot

_Welcome to "Develop With AI Powered Code Suggestions Using GitHub Copilot and VS Code"! :wave:_

GitHub Copilot is an AI pair programmer that helps you write code faster and with less work. It draws context from comments and code to suggest individual lines and whole functions instantly. GitHub Copilot is powered by OpenAI Codex, a generative pretrained language model created by OpenAI.

**Copilot works with many code editors including VS Code, Visual Studio, JetBrains IDE, and Neovim.**

Additionally, GitHub Copilot is trained on all languages that appear in public repositories. For each language, the quality of suggestions you receive may depend on the volume and diversity of training data for that language.

Using Copilot inside a Codespace shows just how easy it is to get up and running with GitHub's suite of [Collaborative Coding](https://github.com/features#features-collaboration) tools.

> **Note**
> This skills exercise will focus on leveraging GitHub Codespace. It is recommended that you complete the GitHub skill, [Codespaces](https://github.com/skills/code-with-codespaces), before moving forward with this exercise.

### :keyboard: Activity: Enable Copilot inside a Codespace

**We recommend opening another browser tab to work through the following activities so you can keep these instructions open for reference.**

Before you open up a codespace on a repository, you can create a development container and define specific extensions or configurations that will be used or installed in your codespace. Let's create this development container and add copilot to the list of extensions.

1. Navigating back to your **Code** tab of your repository, click the **Add file** drop-down button, and then click `Create new file`.
1. Type or paste the following in the empty text field prompt to name your file.
   ```
   .devcontainer/devcontainer.json
   ```
1. In the body of the new **.devcontainer/devcontainer.json** file, add the following content:
   ```
   {
       // Name this configuration
       "name": "Codespace for Skills!",
       "customizations": {
           "vscode": {
               "extensions": [
                   "GitHub.copilot"
               ]
           }
       }
   }
   ```
1. Select the option to **Commit directly to the `main` branch**, and then click the **Commit new file** button.
1. Navigate back to the home page of your repository by clicking the **Code** tab located at the top left of the screen.
1. Click the **Code** button located in the middle of the page.
1. Click the **Codespaces** tab on the box that pops up.
1. Click the **Create codespace on main** button.

   **Wait about 2 minutes for the codespace to spin itself up.**

1. Verify your codespace is running. The browser should contain a VS Code web-based editor and a terminal should be present such as the below:
   ![Screen Shot 2023-03-09 at 9 09 07 AM](https://user-images.githubusercontent.com/26442605/224102962-d0222578-3f10-4566-856d-8d59f28fcf2e.png)
1. The `copilot` extension should show up in the VS Code extension list. Click the extensions sidebar tab. You should see the following:
   ![Screen Shot 2023-03-09 at 9 04 13 AM](https://user-images.githubusercontent.com/26442605/224102514-7d6d2f51-f435-401d-a529-7bae3ae3e511.png)

**Wait about 60 seconds then refresh your repository landing page for the next step.**

---

## 🎓 GitHub Copilot Pro — Student Guide

> **Students get GitHub Copilot Pro for free** through the [GitHub Student Developer Pack](https://education.github.com/pack)!

### What is GitHub Copilot Pro?

GitHub Copilot Pro is the individual tier of GitHub Copilot that gives you an AI pair programmer right in your editor. It offers:

- **Unlimited code completions** — inline suggestions as you type, across dozens of languages.
- **Copilot Chat** — a conversational AI assistant inside VS Code, Visual Studio, JetBrains IDEs, and GitHub.com.
- **Multi-model support** — choose from multiple AI models (including GPT-4o and Claude) for different tasks.
- **Copilot Edits** — make multi-file edits by describing the change you want in natural language.
- **CLI assistance** — get shell command suggestions directly in your terminal with `gh copilot`.

### How Students Get Copilot Pro for Free

1. **Apply for the GitHub Student Developer Pack**
   - Go to [https://education.github.com/pack](https://education.github.com/pack) and click **Get student benefits**.
   - Sign in with your GitHub account and verify your student status (school email address or upload proof of enrollment).
   - Approval typically takes a few days.

2. **Activate GitHub Copilot Pro**
   - Once your Student Developer Pack is approved, navigate to [https://github.com/settings/copilot](https://github.com/settings/copilot).
   - Your free Copilot Pro access is automatically included — no credit card required.

### Setting Up Copilot Pro in VS Code

1. **Install VS Code** — Download from [https://code.visualstudio.com](https://code.visualstudio.com) if you haven't already.
2. **Install the GitHub Copilot extension**
   - Open VS Code and go to the Extensions view (`Ctrl+Shift+X` / `Cmd+Shift+X`).
   - Search for **GitHub Copilot** and click **Install**.
   - Also install **GitHub Copilot Chat** for the conversational assistant.
3. **Sign in to GitHub**
   - When prompted, click **Sign in to GitHub** and authorize the extension.
   - Your Copilot Pro subscription is automatically detected.
4. **Start coding!**
   - Open any file and start typing — Copilot will offer gray inline suggestions.
   - Press `Tab` to accept a suggestion, or `Esc` to dismiss it.
   - Press `Alt+]` / `Option+]` to cycle through alternative suggestions.

### Using Copilot Pro in a GitHub Codespace

GitHub Codespaces gives you a full VS Code environment in your browser — no local setup needed.

1. Click the **Code** button on any repository and select **Create codespace on main**.
2. The GitHub Copilot extension is pre-installed in Codespaces — just sign in and start coding.
3. Use `Ctrl+I` / `Cmd+I` to open **Copilot Edits** for multi-file changes.
4. Use `Ctrl+Shift+I` / `Cmd+Shift+I` to open **Copilot Chat** in the sidebar.

### Key Copilot Pro Features for Students

| Feature | How to use |
|---|---|
| **Inline completions** | Start typing — accept with `Tab` |
| **Copilot Chat** | `Ctrl+Shift+I` in VS Code, or click the chat icon |
| **Explain code** | Select code → right-click → *Copilot: Explain This* |
| **Fix errors** | Hover over a red squiggle → click the lightbulb → *Fix with Copilot* |
| **Generate tests** | Right-click in a file → *Copilot: Generate Tests* |
| **Terminal assist** | Type `@terminal` in Copilot Chat, or run `gh copilot suggest` in your shell ([requires GitHub CLI + `gh extension install github/gh-copilot`](https://docs.github.com/en/copilot/using-github-copilot/using-github-copilot-in-the-command-line)) |
| **Copilot Edits** | `Ctrl+I` to open, describe a multi-file change in plain English |

### Tips for Getting the Most Out of Copilot Pro

- **Write descriptive comments** — Copilot reads your comments as context. Describe *what* you want before you start coding.
- **Use Copilot Chat for explanations** — Ask "What does this function do?" or "Why is this test failing?" directly in the chat.
- **Iterate on suggestions** — If the first suggestion isn't right, press `Alt+]` to see alternatives or refine your comment.
- **Ask for examples** — Prompt Copilot Chat with "Show me an example of a REST API in Express.js" to get working code samples.
- **Keep files focused** — Copilot uses the content of open files as context. Keeping files small and well-organized improves suggestion quality.

### Additional Resources

- 📖 [About GitHub Copilot Individual (Pro)](https://docs.github.com/en/copilot/overview-of-github-copilot/about-github-copilot-for-individuals)
- 🎓 [GitHub Student Developer Pack](https://education.github.com/pack)
- 🚀 [Getting started with Copilot in VS Code](https://docs.github.com/en/copilot/getting-started-with-github-copilot/getting-started-with-github-copilot-in-visual-studio-code)
- 💬 [GitHub Copilot Chat documentation](https://docs.github.com/en/copilot/github-copilot-chat/using-github-copilot-chat-in-your-ide)
- ⚙️ [Configure Copilot settings](https://docs.github.com/en/copilot/configuring-github-copilot/configuring-github-copilot-settings-on-githubcom)
- 🗣️ [Community discussion board](https://github.com/orgs/skills/discussions/categories/code-with-copilot)

---

<footer>

<!--
  <<< Author notes: Footer >>>
  Add a link to get support, GitHub status page, code of conduct, license link.
-->

---

Get help: [Post in our discussion board](https://github.com/orgs/skills/discussions/categories/code-with-copilot) &bull; [Review the GitHub status page](https://www.githubstatus.com/)

&copy; 2023 GitHub &bull; [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [MIT License](https://gh.io/mit)

</footer>
