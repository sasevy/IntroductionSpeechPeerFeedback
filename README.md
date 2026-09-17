# IntroductionSpeechPeerFeedback
# Peer Feedback Tally

A single-page tool for transcribing paper peer-review ballots and turning them into per-student totals. Built for four sections of about 25 students with up to 24 reviewers each.

## Putting it on GitHub Pages

1. Make a new repository on GitHub. Any name works.
2. Upload `index.html` to the root of the repository. The file name matters, so keep it as `index.html`.
3. Go to Settings, then Pages in the left sidebar.
4. Under "Build and deployment," set Source to "Deploy from a branch," pick `main` and the `/ (root)` folder, then Save.
5. Wait a minute or two, then open `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`.

You can also just double-click `index.html` on your own computer and it runs the same way, with no internet needed.

## Where the data lives

Everything stays in the browser you are using, in that browser's local storage. Nothing is uploaded to GitHub or anywhere else, so student names and scores never leave your machine. That has one consequence worth taking seriously: clearing your browser data erases the ballots, and a different computer starts empty.

Use **Download backup** in Setup at the end of each grading session. That gives you a `.json` file you can keep in Drive and load on any other machine with **Load a backup**. The app nags you with a banner once you pass 40 ballots without a backup.

## Entering ballots quickly

Pick a student, then type the four circled scores as digits. The active row advances on its own, so a ballot of 5, 4, 5, 3 is four keystrokes. Press Enter to save and the form clears for the next reviewer.

- `1` through `5` fill the highlighted row
- `Backspace` steps back a row and clears it
- `↑` and `↓` move between rows without scoring
- `Enter` saves the ballot

Comment categories are separate from the scores. Tap them under "Did well" or "Work on" as you read the written comments. Anything the reviewers write that is not on the list yet goes in with the "+ category" button and stays available for every later ballot.

## Getting the numbers out

- **Student** view shows means, sums, the spread of circled scores, the comment tally, and any quoted comments. The Print button gives you a clean page to hand back.
- **Class** view shows the whole section as a table.
- **Summary CSV** exports one row per student with every mean, sum, and comment count.
- **Every ballot CSV** exports the raw rows if you want to run your own analysis.

## Changing the setup

Section names, roster, number of reviewers, scored categories, comment categories, and the list of speeches are all editable in Setup. Re-pasting a roster keeps the ballots of any student whose name is unchanged, so fixing a spelling mid-semester is safe as long as you only change one name at a time.
