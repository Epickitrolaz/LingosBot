# LingosBot

A bot for [lingos.pl](https://lingos.pl) built with Python and Selenium.

---

## 🛠️ Setup & Installation

### Linux

**Prerequisites:**
Ensure you have `python`, `python-pip`, `python-venv`, and `firefox` packages installed on your system.

**Installation:**
1. Clone the repository:
   ```bash
   git clone https://github.com/Epickitrolaz/LingosBot
   cd LingosBot
   ```
2. Make the scripts executable:
   ```bash
   chmod +x setup.sh start.sh
   ```
3. Run the setup script:
   ```bash
   ./setup.sh
   ```
4. Copy the environment template and configure your options:
   ```bash
   cp .env.example .env
   ```
   *(Open `.env` in your text editor and set your email, password, and other variables).*
5. Start the bot:
   ```bash
   ./start.sh
   ```

### Windows

**Prerequisites:**
Ensure you have the latest version of [Python](https://www.python.org/downloads/), [Git](https://git-scm.com/), and [Firefox](https://www.mozilla.org/en-US/firefox/new/) installed.

**Installation Steps:**
1. Open Command Prompt (`cmd`) and navigate to your desired directory (e.g., Desktop).
2. Clone the repository:
   ```cmd
   git clone https://github.com/Epickitrolaz/LingosBot
   cd LingosBot
   ```
3. Run the setup script:
   ```cmd
   setup.bat
   ```
4. Copy the contents of `.env.example` into a new `.env` file, configure your credentials and other variables.
5. Start the bot:
   ```cmd
   start.bat
   ```

---

## ⚙️ Environment Variables

Configure the bot's behavior by editing the `.env` file. Below are the available variables and their usage:

| Variable | Type | Description |
| :--- | :---: | :--- |
| `EMAIL` | `Text` | Your lingos.pl login email. |
| `PASSWORD` | `Text` | Your lingos.pl login password. |
| `LESSON_COUNT` | `Number` | Number of lessons to complete per session. |
| `CHANCE_OF_PASSING` | `Decimal` | Chance of the bot being correct. `1` = correct every time, `3` = correct every 3 questions, etc. |
| `ENABLE_CHALLENGES` | `0/1` | Should the bot automatically select challenges for more points? |
| `AUTOMATED_LOGIN` | `0/1` | Should the bot log in automatically using the provided credentials? |
| `HEADLESS` | `0/1` | Should the browser run in headless mode (hidden window, good for a headless server)? |
| `SCRAPE` | `0/1` | Should the code get the translation list before starting? |
| `APPEND_TO_DB` | `0/1` | Should new words be appended to the local database while running? |
| `LOCKUP_PREVENTION` | `0/1` | Enables the fix to prevent lockups on bad translations. |
| `CLEAR_DB_BEFORE_SESSION`| `0/1` | Removes all database entries before starting a new session. |
| `FORCE_WAIT_SEC` | `Decimal` | **For debugging.** How long the code should wait between actions (in seconds). |
