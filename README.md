# Quiz Game

A browser-based quiz game built with HTML/CSS/JavaScript and hosted on AWS (CloudFront).

## Live Demo
- CloudFront: <https://d10kpdte8q92rn.cloudfront.net/>

## Features
- Multiple topics (STEM, Sports, Geography, History)
- Multiple-choice answers with immediate feedback
- Score tracking + question counter
- Topic UI + menu overlay navigation

## Project Files
- `homeScreen.html` — start screen / topic selection
- `Stem.html`, `Sports.html`, `Geography.html`, `History.html` — quiz pages
- `Style.css` + topic CSS files (`stem_questions.css`, `sports_questions.css`, etc.)

## Improvements / Next Steps
These are planned upgrades to make the project more “production-ready” and portfolio-worthy:

- **Backend high scores**
  - Move `highScores.json` updates to a backend API (ex: AWS Lambda + API Gateway + DynamoDB/S3)
  - Prevents “static hosting can’t write files” limitations and supports real leaderboard persistence

- **Mobile optimization**
  - Improve responsive layout (better scaling for buttons/text box)
  - Support smaller screens + touch interactions (bigger tap targets, spacing, safe areas)

- **Difficulty levels**
  - Easy/Medium/Hard modes
  - Harder questions, fewer hints, shorter timer, etc.

- **Timer**
  - Countdown per question
  - Bonus points for faster answers
  - Auto-skip if time runs out

- **Leaderboard**
  - Dedicated leaderboard screen
  - Top N scores with name + date
  - Filters by topic and/or difficulty

## Notes
This project is hosted as static files via CloudFront. Anything that needs “writing” (like persistent shared high scores)
should be handled through a backend service.
