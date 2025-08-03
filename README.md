# CV Data Extraction using Generative AI – UiPath Project

## Overview
This project automates the process of extracting structured candidate data (e.g., name, email, phone, skills, experience) from unstructured CVs in PDF format using UiPath integrated with a Generative AI model.

## Features
- Reads unstructured CVs in PDF format
- Sends content to a Generative AI (e.g., ChatGPT or Azure OpenAI) via API
- Extracts structured information such as:
  - Name
  - Email
  - Phone number
  - Skills
  - Education
  - Job experience
- Stores the extracted data in Excel or a database
- Handles multiple files in a loop

## Technologies Used
- UiPath Studio
- UiPath PDF Activities
- UiPath HTTP Request Activity
- Generative AI (OpenAI API / Azure OpenAI)
- Excel Automation

## Prerequisites
- OpenAI or Azure OpenAI API Key
- UiPath Studio installed
- Internet connection
- PDFs stored in an input folder

## How It Works
1. The bot reads each PDF CV.
2. It extracts raw text using PDF activities.
3. The text is sent to a Generative AI endpoint with a prompt.
4. The structured response is parsed and stored in Excel or another target.

## Output
Each CV will result in a structured row in Excel or a JSON file with:
- Full Name
- Email Address
- Phone Number
- Address
- Work Experience

## How to Use
1. Update the API key and endpoint in the Config file.
2. Place all CV PDFs in the `/Input` folder.
3. Run the project.
4. Review structured data in the `/Output` folder.

## Security Note
API keys and personal data should be handled securely and not exposed in logs or plain text files.

## Author
This project was created as part of an RPA-AI integration use case to automate document understanding tasks using UiPath and LLMs.

---

For improvements, consider integrating validation steps or extending output to a recruitment platform.
