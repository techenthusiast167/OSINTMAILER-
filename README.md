# OSINTMAILER

A robust Python-based OSINT tool designed for validating and investigating email addresses across social media platforms and known data breaches, enhancing threat intelligence and digital footprint analysis.


# Features

- **Email Validation**: Checks for syntax, disposable status, and MX records.
  
- **Profile Enumeration**: Searches for Gravatar and GitHub profiles.
  
- **Social Media Search Links**: Generates direct search URLs for platforms like Twitter/X, LinkedIn, Instagram, and Facebook.
  
- **Breach & Reputation Checks**: Integrates with HaveIBeenPwned for breach detection and provides a simple email reputation assessment.

- **Google Dorking**: Generates advanced Google search queries for deeper web reconnaissance.
  
- **Reporting**: Outputs results to the console, and generates structured CSV and human-readable PDF reports.

- **Performance**: Utilizes multi-threading for faster checks across various sources.

- **Logging**: Maintains a detailed log of all operations for traceability and debugging (`osint_tool.log`).



# Installation

Copy the tool script via the link https://gist.github.com/techenthusiast167/0f15c12dfaa50e220ac032acdb45ddac and paste it into the nano editor, save it as **osintmailer.py** by pressing (Ctrl+O), Enter, and (Ctrl+X) to exit.




# Install Dependencies:

- Ensure you have Python 3.7+ installed.

- Then, install the required libraries:

      pip install requests dnspython pandas reportlab beautifulsoup4

  (Note: A **requirements.txt** file is not included in a typical Gist where the script is stored, so direct **pip install** is recommended).


# Usage


**Create your Virtual Environment**:

       virtual my_temp_venv
      source my_temp_venv/bin/activate 



**Run the script**:

    python emailosint.py

- Make sure you're in the same directory where you saved the tool.



 **Enter Email**:
 

- When prompted, enter the email address you wish to investigate (e.g., **example@gmail.com**).


 **Review Results**:
 
The tool outputs its findings directly to the console for immediate review.

- Users are encouraged to conduct detailed analysis by exploring the provided **Social Media Search URLs, Google Dork Suggestions, and any discovered GitHub user profile found**, facilitating comprehensive open-source intelligence gathering.

- Additionally, the tool generates two report files in the same working directory for further examination and archival purposes:
  
   **A CSV report**:
  
  `osint_report_example_at_gmail.com.csv`
      
   **A PDF report**:
  
  `osint_report_example_at_gmail.com.pdf`

   **A log file**:

     `osint_tool.log`
   

      



# Purpose of the CSV, PDF Reports, & osint_tool.log


**CSV Report**:

**(osint_report_example_at_gmail.com.csv)**

This file provides a structured, tabular summary of the OSINT findings for the investigated email address. It includes details such as:

- Email validation results (syntax, disposable status)
  
- Presence of profiles on platforms like Gravatar and GitHub

- Data breach indications from HaveIBeenPwned
  
- Email reputation status
  
- Generated social media search URLs
  
- Google dork search URLs for further investigation
  
Because CSV is a widely supported format, users can open it easily in spreadsheet applications (Excel, Google Sheets) or parse it programmatically for additional automated analysis, data aggregation, or reporting.



**PDF Report**:

**(osint_report_example_at_gmail.com.pdf)**

This report provides a human-readable, formatted summary of the data gathered during the OSINT process.
It is designed for:

- Sharing with colleagues or clients in a professional format
  
- Archiving or documenting investigative findings
  
- Quick review without needing spreadsheet software


**osint_tool.log**:

The log file osint_tool.log is used for recording detailed information about the tool’s execution during runtime. Its purpose includes:

- Tracking every step the tool performs, such as checks made (email syntax validation, MX record lookups, breach queries, etc.).
  
- Logging successes, failures, network errors, or unexpected issues encountered during data gathering.
  
- Providing an audit trail to review what happened during an investigation for troubleshooting or verification.
  
- Helping developers diagnose bugs or improve the tool's reliability based on recorded error messages and events.
  
- Maintaining a history of usage that can assist in accountability and debugging without cluttering the console output.
  
- In essence, the log file is a behind-the-scenes record that supports transparency, error detection, and maintenance of the OSINT tool’s operations.

**This is a common practice for professional tooling, where verbose operational details are stored separately from user-facing output to keep the console clean while retaining valuable diagnostic information**.



# How to view the content of the PDF & CSV Reports - Log file:


- On Linux, use **open or xdg-open.**

- Example:

      open osint_report_preciousvincentct_at_gmail.com.pdf

OR 


    xdg-open osint_report_preciousvincentct_at_gmail.com.pdf


- You can also extend using **open** for either **CSV Report** and **osint log** if you want to. 

## Ethical Considerations

-   Always obtain explicit permission before investigating an email address.
  
-   Respect privacy laws and the terms of service of all platforms involved.

-   This tool is intended for lawful, ethical purposes such as security research, digital forensics, or with proper authorization.

## Contributions & Feedback

Feel free to suggest improvements or provide feedback via my Email address or LinkedIn domain:

- preciousvincentct@gmail.com
- http://linkedin.com/in/tech-enthusiast-669279263

  
