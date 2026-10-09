CAT Connect – An App Designed To Help Learners Understand Internet & Network Technologies

The concept behind CAT Connect is a mobile-quiz game, inspired by the classroom favourite, Kahoot!,and built for Grade 10, 11, and 12 learners who do Computer Applications Technology (CAT). It’s set to be based on Network and Internet Technologies topics under the CAPS Curriculum. This game is designed to allow for revision-friendly play among learners. However, instead of working through past papers or constantly browsing over notes, this application will allow a player to answer one multiple-choice question at a time. The application will consist of at least 10 questions that players can answer per game. Each question will offer about 3-4 answer buttons for the player to choose from. The game will provide instant sound and colour feedback after every answer has been chosen, and then it will move on to the next question. At the end of each game, the player’s results will be displayed on the screen, and if they have played the game before, the current score will be compared to the highest score.

The educational goals of this game, in accordance to the Foundations of Game-Based Learning by Plass et al. (2015), are to allow learners to do the following:
-	Be motivated to stay engaged over long periods of time through a series of features that are of motivational nature.
-	Receive a wide range of ways in which they can be engaged in learning.
-	Engage with the game in a way that reflects their specific situation.
-	Receive opportunities for self-regulated learning during playing the game, in which they execute strategies of goal setting, monitoring of goal achievement, and assessment of the effectiveness of the strategies used to achieve the intended goal.

 Besides those educational goals, the other goals of this game are to allow learners, and/or teachers, to do the following:
-	Identify and remember key terminologies under the Network and Internet Technologies sections under the CAPS Curriculum.
-	Distinguish and explain different concepts/ideas under the Network and Internet Technologies section under the CAPS Curriculum.
-	Differentiate between concepts under the Network and Internet Technologies section under the CAPS Curriculum that may be similar and examine their choices for certain questions.
-	Design and add their own questions to the question bank/list on this app, therefore updating the application with the latest content according to the CAPS Curriculum.


 Components Needed For The Game
1.	A phone or tablet to run the CAT Connect App.
2.	A question bank of multiple-choice questions based off Network and Internet Technologies.
3.	Four colour-coded answer buttons.
4.	A 20-second timer for each question.
5.	A score display, a question counter, and a streak counter.
6.	Sound effects for right and wrong answers.
7.	A saved high score.


Setup
1.	Only one player can play the game at a time, but more than one player can be registered on the leaderboard. Players can take turns on the same device and pass it on after each game.
2.	Each player will enter a name on the Home Screen.
3.	The app will set the score, streak, and question number to the starting values at the beginning of each game for each player.
4.	The app will randomly pick questions for each player to answer in each game.


Rules For The Game

1.	Rounds & Questions
-	Each player will have 10 questions to answer per game, and they can only answer one question at a time.
-	Each question will have four answer options, and only one answer will be correct.
-	Each player will have 20 seconds to answer the question.


 2.	Scoring & Streak System
-	The score for each question depends on how quickly the player answers correctly:
	Correct Answer = 500 points + (seconds left * 25 points)
	An instant correct answer would earn an amount close to the maximum of 1000 points, while a correct answer in the last second would earn 525 points.
-	If the player answers 3 or more questions correctly in a row, they will earn an extra 100 points for each further correct answer.
-	The player will get 0 points if:
	The answer is wrong.
	Time runs out before an answer is chosen.
-	If the answer is wrong or time runs out, the streak will reset to 0 and the app shows the correct answer in green.


3.	Moving To The Next Question
-	After an answer is chosen or time runs out, the app will play a sound, show the feedback, and will lock the buttons.
-	After a short pause, the next question will be shown and the timer will reset to 20 seconds.
-	Movement = Question Number + 1


4.	Winning The Game
-	After answering the 10 questions, the Results screen will show the player’s final score.
-	The final score will be compared to the saved high score if there is one. If it is higher, it will become the new high score.


 Initial Algorithm
 
Start

Display Welcome Screen

Set High Score = Saved High Score

~ For Each Player

Display “Player No., Enter Your Name.”

	Input: PlayerName
  
Set Score = 0

Set Streak = 0

Set QuestionNo = 1

~ Randomly Select 10 Questions From The Question Bank

~ For Question Number = 1 To 10

Display QuestionNo And Question

Display AnswerOptions A, B, C, D

Set TimeLeft = 20

Start Timer

~ Repeat Every 1 Second

	TimeLeft = TimeLeft – 1
  
	Display TimeLeft
  
~ Until Player Chooses An Answer Or TimeLeft = 0

~ Stop Timer

~ Disable Answer Buttons

~ If Player Chose An Answer And Answer = CorrectAnswer then

            QuestionPts = 500 + (Time Left × 25)
            
            Streak = Streak + 1
            
 		~ If Streak >= 3 then
    
QuestionPts = Points For Question + 100

Score = Score + QuestionPts

Turn Chosen Button Green

Play Correct Sound

~ Else

QuestionPts = 0

Streak = 0

Turn Chosen Button Grey

Turn Correct Button Green

Play Wrong Sound

EndIf

Display QuestionPts

Display Total Score

~ Wait 1.5 Seconds

QuestionNo = QuestionNo + 1

EndFor

~ Store FinalScore For Player X

~ If FinalScore > HighScore then

HighScore = FinalScore

Save HighScore to TinyDB

Display "New High Score!"

EndIf

Display Final Score and High Score

~ If More Players Remain then

Display "Pass the device to the next player"

EndIf

Display Winner

~ Set Winner = Player With The Highest Final Score

EndIf

Display "Play Again" and "Home" buttons

End



 
