# airat-aibolit-update  
A script for quickly installing and/or updating [ai-bolit](https://revisium.com/ai/), created by Airat Khalitov.

**IMPORTANT:**  
The official website of ai-bolit (https://revisium.com/ai) is no longer accessible, so there are no more official updates.  
The archive contains the last available version.

Since the developers have abandoned this script, it will not detect new vulnerabilities discovered after the last update. (_Unless we decide to maintain and update it ourselves._)

## Installation and Usage:
```bash
git clone https://github.com/AiratTop/airat-aibolit-update

cd airat-aibolit-update

cd ai-bolit

./run-aibolit.sh
```

**Notes:**  
- Place the files you want to scan into the `ai-bolit` directory before running the script `./run-aibolit.sh`.  
- The `./run-aibolit.sh` script sequentially runs two scanning modes: normal (`--mode=1`) and paranoid (`--mode=2`).  
- During scanning, files must be accessible to the script. It’s safer to run it with root privileges.  
- The paranoid mode may produce false positives as it is more sensitive.  
- Detailed usage instructions are provided in the `readme.txt` file, and the changelog can be found in `CHANGELOG.md`.  
