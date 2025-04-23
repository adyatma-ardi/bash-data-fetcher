# bash-data-fetcher

### <b>A. Introduction</b><br>
<b>(A.1) Project Purpose<br></b>
The purpose of this project is to demonstrate how to fetch and process data <br>
using pure Bash scripting. It provides a lightweight, dependency-minimal solution <br>
for accessing APIs, downloading datasets, and automating simple data retrieval tasks <br>
directly from the command line<br><br>
<b>(A.2) Brief Description</b><br>
"<i>bash-data-fetcher</i>" is a collection of reusable Bash scripts designed to interact <br>
with web APIs or public data sources using tools like <i>curl, wget, and jq</i>. The scripts <br>
include functionalities such as:<br>
1. Sending GET requests to RESTful APIs
2. Parsing JSON responses
3. Downloading and saving remote files
4. Scheduling fetch tasks via cron (optional)<br>
  
This project is ideal for those looking to automate data fetching without relying on heavier <br>
programming environments like Python or Node.js.<br><br>
<b>(A.3) Target Users</b><br>
This repository is created for:<br>
- System administrators who need to automate regular data pulls
- Data engineers working in low-resource environments or shell-first systems.
- Developers who want quick CLI tools for API testing and prototyping
- Linux/Bash learners seeking hands-on examples of practical shell scripting 

### <b>B. Installation and Setup</b><br>
<b>(B.1) System Requirements</b><br>
Before installing and using "bash-data-fetcher", ensure your system meets the following minimum <br>
requirements:<br>
Operating System: Linux, macOS, or Windows with WSL<br>
Bash version: 4.0 or higher<br>
Dependencies:<br>
  - curl (for HTTP requests)
  - jq (for parsing JSON)

Memory: At least 1 GB RAM<br>
Storage: At least 100 MB of free disk space<br>
Internet: Required for fetching data from APIs or external sources<br>

Note:<br>
On Native windwos systems (without WSL), it's recommended to use Git Bash or an equivalent terminal that supports Bash scripting.<br>

<b>(B.2) Installation Steps</b><br>
a. Using Terminal (CLI method)
  - Clone the repo:<br>
    ```bash
    git clone https://github.com/adyatma-ardi/bash-data-fetcher.git
    cd bash-data-fetcher
    ```
  - Make the script executable
    ```bash
     chmod +x fetch.sh
    ```
  - (optional) Add to your PATH:
    ```bash
    echo 'export PATH="$PATH:$HOME/bash-data-fetcher"' >> ~/.bashrc
    source ~/.bashrc
    ```
b. Using GitHub Desktop (GUI method)
   1. Clone this repository using GitHub Desktop
   2. Navigate to the folder on your computer
   3. Open your terminal in that directory
   4. Run:
      ```bash
       chmod +x fetch.sh
      ```
<b>(B.3) Initial Configuration</b><br>
1. Create your own config file
   ```bash
   cp .env.example .env
   ```
3. Edit .env to set your preferences
   ```bash
   nano .env
   ```
   ```ini
   API_URL="https://api.example.com/data"
   OUTPUT_FORMAT="json"
   SAVE_TO_FILE="true"
   ```
5. Run a test to check everything's working
   ```bash
   ./fetch.sh --test
   ```
   You should see a "Connection successful!" or sample output on your terminal

### <b>C. Project Structure 🗂️</b><br>
This section outlines the structure of the "bash-data-fetcher" project so you<br>
can easily navigate and understand its components. <br>
<b>(C.1) Explanation of Main folders and Files</b><br>
  1. fetch.sh : The main executable Bash script that handles data fetching logic.This is the entry point of the project
  2. .env.example : Template for environment variables (API URL, output format, etc). Copy it to .env to configure
  3. .env : your actual configuration file (ignored by Git). Used for customizing fetch behavior
  4. utils/ : contains helper scripts (e.g., data cleaning, formatting functions) to keep fetch.sh clean
  5. logs/ : stores log files generated from fetch runs for debugging or auditing
  6. output/ : output folder where fetched data (JSON/CSV/etc.) is saved, if SAVE_TO_FILE=true
  7. README.md : the documentation file you're reading right now. Includes setup and usage instructions.
  8. LICENSE : the license file for the project
  9. .gitignore: specifies which files/folders Git should ignore (like .env, logs/, etc).

<b>(C.2) Project Structure Diagram</b><br>
Here's a simplified overview of how the project is organized
bash-data-fetcher/
│<br>
├── fetch.sh                # 🔧 Main script<br>
├── .env.example            # 🧪 Sample environment config<br>
├── .env                    # ⚙️ Actual user config (ignored by Git)<br>
├── README.md               # 📖 Documentation<br>
├── LICENSE                 # 📜 License info<br>
├── .gitignore              # 🚫 Git ignore rules<br>
│<br>
├── utils/                  # 📦 Utility functions<br>
│   └── format_output.sh    # Example: output formatting script<br>
│<br>
├── logs/                   # 📝 Runtime logs<br>
│   └── fetch-2025-04-23.log<br>
│<br>
└── output/                 # 📁 Fetched data<br>
    └── result_001.json<br>




