# CAT Connect

A Kahoot-style mobile quiz on **Network Technologies** and **Internet Technologies** for Grade 10-12 Computer Applications Technology (CAT) learners, aligned to the CAPS curriculum. Built with MIT App Inventor and released as an Open Educational Resource (OER).

![Home screen](screenshots/home.jpg)
![Quiz screen](screenshots/quiz.jpg)
![Results screen](screenshots/results.jpg)
![How To screen](screenshots/howto.jpg)
![OER/About screen](screenshots/oer.jpg)

## Target audience

- Grade 10-12 CAT learners revising for tests and exams
- CAT teachers who want a free, editable revision tool

## How to play

1. Enter your name and tap **Play**.
2. Answer 10 randomly chosen questions. You have 20 seconds for each.
3. Tap the colour button with the correct answer.
4. Faster answers earn more points: 500 base points plus 25 points for every second left (up to about 1,000).
5. Three or more correct answers in a row earn a 100-point streak bonus.
6. A wrong answer or running out of time scores 0.
7. At the end, your score is compared with your saved high score.

## How to install

1. Download `CATConnect (1).apk` from the main page.
2. Open the file on your Android phone or tablet.
3. If asked, allow **Install from unknown sources** in your settings.
4. Open **CAT Connect** and play.

## How to edit and remix

1. Download `CATConnect.aia`.
2. Go to [appinventor.mit.edu](https://appinventor.mit.edu) and sign in with a Google account.
3. Choose **Projects > Import project (.aia) from my computer**.
4. Open **QuizScreen** and click **Blocks**.
5. Edit the global lists `questions`, `optA`, `optB`, `optC`, `optD` and `answers`.
   - Item 1 in every list belongs to question 1, item 2 to question 2, and so on.
   - In `answers`, use 1 for A, 2 for B, 3 for C and 4 for D.
   - Every list must have the same number of items.
6. Connect with **Connect > AI Companion** to test, then use **Build > Android App (.apk)** to create your own installable file.



## Repository contents

| Folder / file | Description |
|---|---|
| `CATConnect.aia` | Source project for MIT App Inventor |
| `CATConnect (1).apk` | Installable Android app |
| `screenshots/` | Images of the app |
| `docs/` | Planning document |
| `media/` | Logo and sound files |
| `LICENSE` | CC BY 4.0 licence text |

## Licence

This work is licensed under the **Creative Commons Attribution 4.0 International Licence (CC BY 4.0)**.

You may share and adapt this work for any purpose, including commercially, as long as you give appropriate credit to Patrick Mokwena, provide a link to the licence, and indicate if changes were made.

Licence details: https://creativecommons.org/licenses/by/4.0/

| Built with | MIT App Inventor | https://appinventor.mit.edu | |

## Curriculum

Content is aligned to the CAPS Computer Applications Technology (CAT) curriculum, topics **Network Technologies** and **Internet Technologies**. Teachers should check the question bank against the current CAPS document for their grade.

## Author

Patrick Mokwena, North-West University, October 2026
Contact: 56042345@mynwu.ac.za

## Suggested citation

Mokwena, P.T. (2026) *CAT Connect: a quiz on network and internet technologies* [Mobile application]. Available at: https://github.com/pmokwena/CAT-Connect (Accessed: ).
