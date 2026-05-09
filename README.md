# SSDD-CCA
MediSafe Telemedicine Platform – CCA Submission

This project demonstrates secure software design by implementing:
- A vulnerable version with 3 security flaws:
  1. IDOR (Insecure Direct Object Reference)
  2. Video session reuse
  3. Token leakage

- A fixed version where all vulnerabilities are resolved.

How to run:

1. Install dependencies:
   pip install -r requirements.txt

2. Run vulnerable version:
   python -m uvicorn vulnerable_version.app:app --reload

3. Run fixed version:
   python -m uvicorn fixed_version.app:app --port 8001 --reload

4. Run tests:
   pytest tests/test_security_vulnerable.py
   pytest tests/test_security_fixed.py

Note:
Add your screenshots in the Screenshots folder and your project code in the Source_Code folder before submission.
