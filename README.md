# LinkedIn-Auto-Job-Applier
This is a web automation bot designed to streamline the job application process on LinkedIn. It automatically searches for jobs that match your profile, fills out application forms, tailors your resume based on job-specific details—such as required skills, job description, and company information—and submits applications on your behalf. The bot can apply to over 100 jobs in under an hour.

# How to Configure the Bot

Personal Details
Open the personals.py file located in the /config folder.
Enter your personal information such as name, phone number, address, etc. These details will be automatically filled in during job applications.

Application Questions
Open the questions.py file in the /config folder.

Provide your answers to common job application questions.

Configure options such as whether the bot should pause before submitting applications or stop when it encounters unanswered or unknown questions.

Job Search Preferences
Open the search.py file in the /config folder.

Set your job search preferences and filters (e.g., job title, location, experience level).

These settings determine which jobs the bot will apply to or skip.

Login Credentials & Resume Generation (Optional)
Open the secrets.py file in the /config folder.

Enter your LinkedIn username and password for automatic login.

Provide your OpenAI API key if you want the bot to generate customized resumes and cover letters.

If you leave the username or password blank (or keep the default), the bot will try to log in using your saved browser profile. If login fails, you’ll be prompted to log in manually.

Bot Behavior & Settings
Open the settings.py file in the /config folder to customize the bot’s behavior:

Keep the screen awake

Set randomized click intervals (to mimic human behavior)

Enable background mode or stealth mode to reduce the chance of detection

Adjust other operational preferences as needed

Resume Setup (Optional)
Add your default resume file at the path specified in the default_resume_path variable inside questions.py, for example:

default_resume_path = "all resumes/default/resume.pdf"


If not provided, the bot will use the most recent resume you've submitted on LinkedIn.
(In development: Automatic resume generation using OpenAI API if no resume is supplied)

▶️ Running the Bot

To start the application bot, run:

python runAiBot.py


Sit back and let the automation begin.

To access your Applied Jobs history via the user interface:

python app.py


Then open your web browser and navigate to:
http://localhost:5000
