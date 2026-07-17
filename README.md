Resume Data Extraction with Regex

A regex and pandas project that parses a dataset of 1,352 resumes and pulls out structured candidate data: job title, technical skills, and highest education level. Built as a mock HR analytics task, where the goal is turning messy resume text into a clean, filterable table of tech-focused candidates.

What it extracts


job_title — the most recent job title, pulled from the header line at the top of each resume
tech_skills — mentions of Python, SQL, R, and Excel, found using word-boundary regex matching
education — the highest degree found in each resume (PhD > Master > Bachelor)


Resumes missing any of the three fields are dropped, so the final dataset only contains complete records.

Result

1,352 resumes narrowed down to 181 complete candidate records with a job title, at least one tech skill, and an education level all identified.

Tools

Python, pandas, re

Files


notebook.ipynb — full extraction and cleaning process
resumes.csv — source dataset
