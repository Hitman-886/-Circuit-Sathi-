# Circuit Sathi

Circuit Sathi is a lightweight, local web application that converts electronics notes into interactive multiple-choice questions (MCQs). Just paste your notes, and it instantly generates practice quizzes to test your knowledge without needing an internet connection.

## Who I built it for
I built this for a classmate who is preparing for their electronics exams and needed an easy way to self-test on study materials.

## How to run it
1. Install [LM Studio](https://lmstudio.ai/).
2. Download a small Gemma model (e.g., 1B or 4B parameter model in Q4 format) through the LM Studio app.
3. Open the **Developer** tab in LM Studio.
4. Start the local server (it usually runs on `http://localhost:1234/v1`).
5. Check the box to turn ON **"Enable CORS"**.
6. Double-click the `index.html` file to open it in your browser.

## Open-source AI & Why local matters
This project uses open-weight models like **Gemma**. Running the model locally matters because:
* It works completely offline.
* Your study notes stay securely on your laptop.
* There is zero API cost.
* You can easily swap to other open-source models as they are released.

## Troubleshooting
* **Server not reachable:** Ensure LM Studio is open, the Developer server is started, and "Enable CORS" is checked. Check if the port is `1234`.
* **Model returns bad JSON:** Smaller models sometimes struggle with formatting. If this happens, simply try clicking "Make questions" again, or use a slightly larger model (like 4B or 8B) if your laptop can handle it.

---
*Built with help from AI tools*
*Built for the Hacktoberfest 2026 Weekend Challenge: Build for a Friend*
