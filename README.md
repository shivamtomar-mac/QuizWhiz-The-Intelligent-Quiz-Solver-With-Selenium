# QuizWhiz-The-Intelligent-Quiz-Solver-With-Selenium


5.1 Login and Initial Navigation

When QuizWhiz is launched, the application starts Chrome WebDriver, which will be an emulator. the automatic browser. QuizWhiz navigates to the Moodle website, where it interacts with the login page by locating the username and password fields. After entering the user's credentials, it submits the login form, granting access to the user’s Moodle dashboard. 

• System Action: QuizWhiz retrieves the username and password fields using Selenium’s find_element method, simulates typing the user’s login credentials, and clicks the login button to proceed.

• User Experience: Users simply launch the program without needing to navigate or manually input credentials, saving time and effort.

![image](https://github.com/user-attachments/assets/5594771c-4e08-475c-8964-9e666274255b)

                      Fig. 5.1 QuizWhiz Login Process on Moodle


5.2 Detecting Available Quizzes 

Once logged in, QuizWhiz examines the Moodle dashboard for any ongoing or available quizzes. This is achieved by locating elements that contain the text "Attempt quiz now," which signals active quizzes. If no quiz is available, the system informs the user and terminates gracefully.

• System Action: Selenium scans the page for active quiz elements and identifies the first available quiz to attempt.

• User Experience: Users are notified immediately if there are no active quizzes, allowing them to focus on other tasks without having to check manually.

![image](https://github.com/user-attachments/assets/e49c617a-d8a3-458c-b4f4-3ca8eaf5de51)

                       Fig. 5.2 Detection of Available Quizzes


5.3 Starting the Quiz

After detecting an available quiz, QuizWhiz initiates the attempt by navigating to the quiz page. 
It clicks the necessary buttons to start the quiz and proceeds to the first question.

•          System Action: Selenium handles all button interactions, from initiating the quiz 
attempt to clicking "Start attempt" and confirming the action.

•          User Experience: Users experience a completely automated process as the system
handles each stage of quiz initiation autonomously.

![image](https://github.com/user-attachments/assets/3f3ab761-a79a-4e36-8e33-f2241d22f861)

              Fig. 5.3 Quiz Start

