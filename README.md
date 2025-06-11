# GitHub Finder

> A sleek web application to search for GitHub users, view their profiles, and explore their repositories with repo stats, language breakdown, and pagination.

---

## Aim

To build a responsive and interactive web tool that leverages the GitHub API to fetch and display detailed information about any GitHub user and their repositories.

---

## Objectives

- Search for any GitHub user using a clean UI  
- Display user profile details like avatar, bio, location, company, etc.  
- List latest repositories with stars, watchers, forks  
- Show repository language as colored badges  
- Implement pagination for repositories  
- Enable smooth API integration and responsive design

---

## Tech Stack

| Layer         | Tech Used                  |
|--------------|----------------------------|
| **Frontend**  | HTML5, CSS3, Bootstrap 5   |
| **Logic**     | Vanilla JavaScript (ES6+)  |
| **API**       | GitHub REST API v3         |
| **Tooling**   | VS Code, Git, GitHub       |

---

## How It Works

1. User types a GitHub username in the input field and clicks **Search**.
2. App fetches user data and latest repositories using GitHub API.
3. User profile is displayed with badges for public stats.
4. Repositories are shown with stars, watchers, forks, and **language badges**.
5. If more than 5 repos, **pagination** buttons (Next/Previous) allow browsing.
6. Graceful error handling for "User not found" and network issues.

---

## Features

- Responsive Bootstrap 5 layout  
- API data fetch with `async/await`  
- Reusable `Github` and `UI` classes  
- Loader animation while fetching  
- Pagination for repo lists  
- Language tag on each repository  

---

## Future Scope

- Add dark/light mode toggle  
- Display language breakdown as a pie chart (using Chart.js)  
- 🕵️Display total contribution stats using GitHub GraphQL API  
- Add filters (e.g., sort repos by stars, language)  
- Recent search history stored in localStorage  
- Convert to a PWA (Progressive Web App)  

---

## Challenges Faced

- Handling GitHub API rate limits (especially without OAuth)  
- Designing clean pagination logic without backend state  
- Parsing and displaying dynamic data (some users have `null` fields)  
- Keeping the UI minimal yet informative  
- Ensuring the code stays modular and clean (with separate files)