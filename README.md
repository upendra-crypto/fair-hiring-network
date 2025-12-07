Fair Hiring Network

This is a small prototype project to promote fair and skill-based hiring.
It avoids biased filtering and instead focuses on verified skills.

Features

✔ Candidates can enter their skills
✔ Recruiters can post jobs
✔ System matches candidates with jobs
✔ Shows score and explanation
✔ Detects bias in selections
✔ Login system with roles

Roles

Candidate

Register & submit skill levels

Can be selected through matching

Recruiter

Create job requirements

View matched candidates

Tech Used

Backend → FastAPI (Python)

Frontend → HTML, JavaScript

Authentication → JWT tokens

Styling → Basic CSS

How to Run
Backend:
cd backend
pip install fastapi uvicorn python-jose passlib[bcrypt]
uvicorn main:app --reload


Runs at:
http://127.0.0.1:8000

Frontend:

Open this file in browser:

frontend/index.html


OR run local server:

cd frontend
python -m http.server 5500


Open browser → http://localhost:5500

Sample Login Workflow
Signup:

POST /signup with:

email, password, role

Login:

POST /login → system returns a token.

Use this token for protected APIs:

Authorization: Bearer <token>

Future Improvements

🔹 Save data in a real database
🔹 Add resume scanning
🔹 Code skill tests
🔹 Advanced recommendation
