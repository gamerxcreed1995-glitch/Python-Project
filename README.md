A command-line based quiz management system built in Python. It supports two roles: Faculty and Student, enabling quiz creation, participation, and performance analytics with graphical visualization.

Source code:

Features
Faculty
Create quizzes with multiple questions and options
View analytics:
Total attempts
Average, highest, lowest scores
View total attempt count
Visualize student performance using graphs
Student
View available quizzes
Attempt quizzes
Get instant scores
Tech Stack
Python 3
JSON (for data storage)
Matplotlib (for graphs)
File Structure
project/
│
├── main.py          # Main application script
├── users.json       # Stores user credentials
├── quiz.json        # Stores quizzes
├── results.json     # Stores quiz results
Installation
Clone the repository:
git clone https://github.com/your-username/quiz-system.git
cd quiz-system
Install dependencies:
pip install matplotlib
Running the Project
python main.py
Default Login Credentials
Role	Username	Password
Faculty	faculty1	123
Faculty	faculty2	123
Student	student1	123
Student	student2	123
How It Works
Startup
Initializes JSON files if not present
Login System
Authenticates users based on stored credentials
Role-Based Access
Faculty → Quiz creation + analytics
Student → Quiz attempts
Data Storage
All data stored locally in JSON files
Graph Visualization
Uses Matplotlib to display student performance trends
Key Functions
setup() → Initializes files
login() → Handles authentication
create_quiz() → Faculty creates quizzes
attempt_quiz() → Student attempts quiz
view_analytics() → Displays stats
student_graph() → Shows performance graphs
Future Improvements
GUI version (Tkinter / Web app)
Timer-based quizzes
Leaderboard system
Question randomization
Secure password handling
Notes
Data is stored locally (not suitable for production use)
Graphs open in separate windows
Input validation is basic
