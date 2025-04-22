# bash-data-fetcher

### <b>Introduction</b><br>
<b>(A) Project Purpose<br></b>
The purpose of this project is to demonstrate how to fetch and process data <br>
using pure Bash scripting. It provides a lightweight, dependency-minimal solution <br>
for accessing APIs, downloading datasets, and automating simple data retrieval tasks <br>
directly from the command line<br><br>
<b>(B) Brief Description</b><br>
"<i>bash-data-fetcher</i>" is a collection of reusable Bash scripts designed to interact <br>
with web APIs or public data sources using tools like <i>curl, wget, and jq</i>. The scripts <br>
include functionalities such as:<br>
1. Sending GET requests to RESTful APIs
2. Parsing JSON responses
3. Downloading and saving remote files
4. Scheduling fetch tasks via cron (optional)<br>
  
This project is ideal for those looking to automate data fetching without relying on heavier <br>
programming environments like Python or Node.js.<br><br>
<b>(C) Target Users</b><br>
This repository is created for:<br>
- System administrators who need to automate regular data pulls
- Data engineers working in low-resource environments or shell-first systems.
- Developers who want quick CLI tools for API testing and prototyping
- Linux/Bash learners seeking hands-on examples of practical shell scripting 

### <b>Installation and Setup</b><br>
<b>(A) System Requirements</b><br>
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

<b>(B) 🚀 Installation Steps</b><br>
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
      <br>
### <b>Initial Configuration</b><br>
   1. Create yout ow
   2. Navigate to the folder on your computer
   3. Open your terminal in that directory
   4. Run:
      ```bash
       chmod +x fetch.sh
      ```

(A) 🔍 Project Purpose<br>
(A) 🔍 Project Purpose<br>
(A) 🔍 Project Purpose<br>
(A) 🔍 Project Purpose<br>
