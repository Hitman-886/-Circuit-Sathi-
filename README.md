# Circuit Sathi

Circuit Sathi is a lightweight, local web application that converts electronics notes into interactive multiple-choice questions (MCQs). Just paste your notes, and it instantly generates practice quizzes to test your knowledge without needing an internet connection.

## Who I built it for
I built this for a classmate who is preparing for their electronics exams and needed an easy way to self-test on study materials.

## How to run it
1. Install Ollama from [ollama.com](https://ollama.com).
2. Open Command Prompt and run: `ollama pull gemma3:4b`
3. Set the environment variable `OLLAMA_ORIGINS` to `*` (Search Windows for "environment variables" > Edit for your account > New), then fully Quit and reopen Ollama.
4. Double-click `index.html` to open the app.

## Open-source AI & Why local matters
This project uses open-weight models like **Gemma** running fully offline through **Ollama**. Running the model locally matters because:
* It works completely offline.
* Your study notes stay securely on your laptop.
* There is zero API cost.
* You can easily swap to other open-source models as they are released.

## Troubleshooting
* **Server not reachable:** Ensure Ollama is running, the `OLLAMA_ORIGINS` environment variable is set to `*` (and you fully quit/restarted Ollama after setting it), and a model is pulled. Check if the port is `11434`.
* **Model returns bad JSON:** Small models like 4B sometimes output malformed JSON (like missing brackets). If you get a "failed to parse JSON" error or similar, it is a known limitation of small local models—simply click the "Make questions" button again.

---
*Built with help from AI tools*
*Built for the Hacktoberfest 2026 Weekend Challenge: Build for a Friend*
