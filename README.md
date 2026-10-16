# Module 2: `.gitignore` & Amending Commits

## Part 1: `.gitignore`

* **What it does:** Tells Git which files or folders to completely ignore (passwords, junk files, heavy libraries).
* **How to set it up:**
  * Create a file named `.gitignore` in your project folder.
  * List files/folders to hide, one per line (e.g., `.env`, `node_modules/`).
* **If a file is already being tracked:**
  * Run `git rm --cached <filename>` to stop tracking it without deleting the actual file.

## Part 2: `git commit --amend`

* **What it does:** Fixes or updates your **very last** commit instead of creating a new one.
* **Fix a typo in your last commit message:**
  * Run: `git commit --amend -m "Your new message"`
* **Add a forgotten file to your last commit:**
  * Stage the file: `git add <filename>`
  * Combine it into the last commit: `git commit --amend --no-edit`
* **Golden Rule:** Only amend commits on your local machine—don't amend after pushing code to GitHub!
