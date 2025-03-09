
# EPAI-v5 Capstone - Agentic Python

EPAI-V5 - Extensive Python & PyTorch for AI -(Version 5), is an advanced Python course for fundamental understanding of Python Language and the PyTorch library. Designed for those who want to become application and ML Architects, offered by [The School of AI](https://theschoolof.ai/)


## Project Overview
This capstone aims to make use of all the python concepts coveres in the course so far, while also introducing the students to the concept of Agentic AI. The project involves writing some python utility modules, that provide automated email workflows, calender integration and file management capabilities. ANd also using LLM models (Gemini) that are used to understand the uesr instructions and pick the appropriate tools from the utility toolset and generate a code that caters to the user prompt. 

Here are the instructions for the capstone: 

Your go-to model is Gemini-2.0-flash-exp. It's free for the usage you're going to have. Build an agent that: 
scans a folder, 
- identifies file types 
- moves them into categorized folders (e.g., PDFs, images, code files, etc) 
- uses online services to compress PDF 
- uses online services to compress PNGs and JPGs 
- reads a particular file called "todo.txt" and performs these tasks if mentioned inside: 
    - Remind me to "------" via email 
    - Add a calendar invite for "" date and share it with "--@--.com" 
    - Share the stock price for NVIDIA every day at 5 PM via email with me 
    - more if you wish 

Restriction:
You CANNOT use any LLM for any of the tasks mentioned directly. Your LLM use is to call a python function that does these jobs!
You need to show the start-to-end of all 6 tasks in a YouTube video
Submission:
Link to the YouTube video
Link to the GitHub Code

### Key Features
- **Email Automation**
  - Decorator-based email sending with SMTP configuration and error handling
  - Reminder emails and calendar invite generation with ICS attachments
  - Scheduled daily stock price emails using background scheduler

- **File Management**
  - Recursive directory scanning and file type categorization
  - File organization by extension with automatic folder creation
  - ZIP archive creation for files/folders with error handling

- **Stock Monitoring**
  - Real-time stock price lookup using Yahoo Finance
  - Scheduled daily price updates with configurable timing

Deviation from requirement - A text box with customisable task prompt from user has been implemented, in place of reading and parsing the todo.txt file

### Installation & Usage
```bash
# Install dependencies
pip install requirements.txt
```

### Environment Variables
Required for email features:
```env
SENDER_EMAIL=your_email@gmail.com
SENDER_PASSWORD=your_app_password
MY_GOOGLE_API_KEY=google_key_gor_gemini_model
```

### Dependencies
- yfinance - Stock price data
- apscheduler - Background scheduling
- smtplib - Email sending
- os/shuutil - File operations

### Contribution
Please ensure new features maintain the existing decorator pattern and include:
- Comprehensive docstrings
- Environment variable configuration where needed
- Error handling in decorated functions
- Type hinting for public methods
```// End Generation Here
```
