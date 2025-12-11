The Forensic Integrity Sentinel is an automated triage system designed for rapid incident response. It leverages Google Gemini 2.5 Flash to analyze raw, unstructured volatile data artifacts (RAM/Registry dumps) and instantly transform them into a comprehensive, standardized, and machine-readable JSON Incident Report and a Human-Readable Summary.
This approach drastically reduces the time required for initial forensic deduction, replacing hours of manual log parsing with seconds of AI-driven analysis and structured reporting.
To run the Forensic Integrity Sentinel on your machine, follow these steps:
1. Prerequisites
Python 3.8+
A Gemini API Key (set as an environment variable)
Setup and Installation

Clone the repository:

git clone https://github.com/your-username/gemini-forensic-triage-automator.git
cd gemini-forensic-triage-automator

Install dependencies:
pip install -r google-genai

Execution
The project reads the sample data from the included file: data/forensic_artifacts_sample.txt.

Ensure your API Key is set:
export GEMINI_API_KEY='YOUR_API_KEY_HERE'

Run the main script:
python forensic_sentinel.py

4. Expected Output
The script will print the human-readable summary to the console and save the two required output files in the root directory:

CoC_IR-IR-2025-09-08-044.json
CoC_IR-IR-2025-09-08-044.txt
