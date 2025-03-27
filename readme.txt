AI-BOLIT Scanner Documentation (English Translation)

The AI-BOLIT scanner is designed to check websites for malware and hacking. It can be used both preventively for regular malware scans and to detect hacker shells, backdoors, phishing pages, malicious injections, doorway pages, spam links, and other harmful fragments in website files.

The scanner can be run either directly on the hosting server (it is recommended to run the scanner in command-line mode via SSH) or on a local computer under MacOS X or *nix operating systems. AI-BOLIT checks files using its proprietary antivirus database and employs heuristic rules to detect new (previously unknown) malicious fragments. When harmful fragments are detected, the scanner generates a report listing the identified files in HTML or plain text format.

The scanner has two modes: "Normal" and "Paranoid."

To diagnose hacking and infection, it is sufficient to scan the website files in "Normal" mode. This mode provides accurate results without false positives and is suitable for assessing whether the website is infected or compromised. To thoroughly check the website for viruses and hacker scripts and generate a report for cleaning, the files should be scanned in "Paranoid" mode. This mode includes not only known malicious fragments or hacker scripts but also suspicious fragments that need to be reviewed as they may potentially be harmful.

Sometimes, the same code fragments may be used in both hacker scripts and legitimate CMS scripts. Therefore, it is impossible to automatically determine 100% whether a file is malicious. Such files will be displayed in the report and must be manually reviewed to assess their safety.

---

Remember that even one overlooked shell or backdoor can lead to repeated hacking and infection of the website. Therefore, when cleaning a website, use the report generated in "Paranoid" mode and thoroughly check all files marked in red in the report.

If you are running the scanner in command-line mode, you can set the mode number using the --mode parameter.

php ai-bolit.php --mode=1 - Normal mode (diagnosis)  
php ai-bolit.php --mode=2 - Paranoid mode (for cleaning)

Refer to the instructions on the following pages:

https://revisium.com/kb/ai-bolit-console-faq.html  
https://revisium.com/kb/ai-bolit-masterclass.html

---

Quick Scan (not recommended for cleaning the website):

1. Open the file /ai-bolit/ai-bolit.php and find the line  
   define('PASS', '....

   Replace the second set of apostrophes with your password, e.g., Mypass16:  
   define('PASS', 'MyPass234');

2. Copy the files from the /ai-bolit/ folder to the root directory of the server.

3. Open your browser and navigate to:  
   https://your_site/ai-bolit.php?p=MyPass234  
   Wait for the report to generate.

4. After viewing the report, delete the AI-BOLIT files and the script from the website.

If something goes wrong, refer to the FAQ: https://revisium.com/ai/faq.php

---

Full Scan (recommended):

1. Copy the files from the /ai-bolit/ folder to the root directory of the server.

2. Connect to the server via SSH and navigate to the website folder.

3. Run the following command in the terminal:  
   php ai-bolit.php

4. Wait for the scan to complete.

5. Copy the generated report file AI-BOLIT-REPORT-<date>-<time>.html from the server to your local machine.

If something goes wrong, refer to the FAQ: https://revisium.com/ai/faq.php

---

Additional Resources:

https://revisium.com/ru/products/antivirus_for_ispmanager/ - Antivirus for ISPmanager Lite  
https://revisium.com/ru/products/antivirus_for_ispmanager/ - Antivirus for Plesk Onyx  

https://revisium.com/ai/ - Official AI-BOLIT Page  
https://revisium.com - Website Security and Protection  
https://revisium.com/blog/ - Revisium Blog  
http://vk.com/siteprotect - VK Group  
http://twitter.com/revisium - Twitter @revisium  
https://www.facebook.com/Revisium - Facebook Page  
