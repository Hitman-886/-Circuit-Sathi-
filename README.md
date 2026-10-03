# Circuit Sathi

Circuit Sathi is a lightweight, local web application that converts electronics notes into interactive multiple-choice questions (MCQs). Just paste your notes, and it instantly generates practice quizzes to test your knowledge without needing an internet connection.

## Who I built it for
I built this for a classmate who is preparing for their electronics exams and needed an easy way to self-test on study materials.

## How to run it
1. Install Ollama from [ollama.com](https://ollama.com/).
2. Open your terminal and run: `ollama pull gemma3:4b`
3. Set the environment variable `OLLAMA_ORIGINS` to `*` so the browser can connect. On Windows:
   - Search for "environment variables" in the Start menu.
   - Click **Edit environment variables for your account**.
   - Click **New** and add `OLLAMA_ORIGINS` as the name and `*` as the value.
4. Quit and reopen Ollama so it picks up the new environment variable.
5. Double-click the `index.html` file to open it in your browser.

## Open-source AI & Why local matters
This project uses open-weight models like **Gemma** running fully offline through **Ollama**. Running the model locally matters because:
* It works completely offline.
* Your study notes stay securely on your laptop.
* There is zero API cost.
* You can easily swap to other open-source models as they are released.

## Troubleshooting
* **Server not reachable:** Ensure Ollama is running, the `OLLAMA_ORIGINS` environment variable is set to `*` (and you restarted Ollama after setting it), and a model is pulled. Check if the port is `11434`.
* **Model returns bad JSON:** Smaller models sometimes struggle with formatting. If this happens, simply try clicking "Make questions" again, or use a slightly larger model if your laptop can handle it.

---
*Built with help from AI tools*
*Built for the Hacktoberfest 2026 Weekend Challenge: Build for a Friend*
