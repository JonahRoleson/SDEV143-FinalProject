# SDEV143 Final Project
---
## Git & GitHub Workflow Overview

This repo demonstrates the basics of creating, linking, and collaborating on Git projects.

1. Establish your repository
# Create a new local folder and initialize it
<pre>```
mkdir my-project
cd my-project
git init
```</pre>


Update your GitHub profile (add profile pic, bio, etc.) via the GitHub website
.

2. Create a .gitignore file
<pre>```
echo "__pycache__/" >> .gitignore
echo "*.log" >> .gitignore
git add .gitignore
git commit -m "Add .gitignore"
```</pre>

3. Create a repository on GitHub (public)

Go to GitHub → “New Repository” → name it my-project → Public.

Copy the repo URL (HTTPS or SSH).

4. Link local and remote repositories
<pre>```
git remote add origin https://github.com/<username>/my-project.git
git branch -M main
git push -u origin main
```</pre>

5. Commits – The Three States

Modified → You edit a file:

<pre>```
echo "Hello World" >> hello.txt
```</pre>


Staged → Add file to staging:

<pre>```
git add hello.txt
```</pre>


Committed → Save a snapshot:

<pre>```
git commit -m "Add hello.txt"
```</pre>

6. Push changes to GitHub
git push origin main

7. Pull Requests (Scenario)

On GitHub, create a new branch (e.g., feature-update).

Push changes from local:

<pre>```
git checkout -b feature-update
echo "New feature text" >> feature.txt
git add feature.txt
git commit -m "Add feature text"
git push origin feature-update
```</pre>


Open a Pull Request on GitHub: feature-update → main.

8. Issues (Teamwork)

Go to Issues tab → Create a new Issue.

Assign the Issue to your classmate.

Add a comment to discuss it.

Example: “Update README with project goals.”

9. Team Updates

Update a designed file:

<pre>```
echo "Team update line" >> design.txt
git add design.txt
git commit -m "Team update to design.txt"
git push
```</pre>


Add a new file:

<pre>```
echo "New file content" >> newfile.txt
git add newfile.txt
git commit -m "Add new file"
git push
```</pre>

10. Branching for Features
<pre>```
git checkout -b new-feature
echo "Temporary info" >> temp.txt
git add temp.txt
git commit -m "Add temporary info"
git push origin new-feature
```</pre>


Later, this branch can be removed after merging.
