GitHub Commit and Branch Example
================
David Kang
2025-10-23

- [First Commit](#first-commit)
- [Second Commit](#second-commit)
- [Branches](#branches)
- [Summary](#summary)

# First Commit

This section represents the **first commit** of your project.

Typical contents: - Initial project setup - Adding `.gitignore` -
Creating a basic `README.md` - Initializing Git with `git init` add an
edit another line added

``` r
# Terminal commands
mkdir my-project
cd my-project
git init
echo "# My Project" > README.md
git add .
git commit -m "Initialize project with basic structure"
```

------------------------------------------------------------------------

# Second Commit

This section corresponds to your **second commit**, where you add your R
Markdown file and test output.

``` r
# Add example R Markdown file
touch example_github_doc.Rmd

# Stage and commit
git add example_github_doc.Rmd
git commit -m "Add example R Markdown file for GitHub document output"
```

------------------------------------------------------------------------

# Branches

You can create and test changes safely in separate branches.

``` r
# Create and switch to a test branch
git checkout -b test-doc-output

# Make changes, then commit
git add .
git commit -m "Test rendering of R Markdown output"

# Merge back to main when ready
git checkout main
git merge test-doc-output
```

**Common branch names:** - `main` → stable production branch  
- `test-doc-output` → for testing `.Rmd` output  
- `feature-rmd-template` → for adding R Markdown features

------------------------------------------------------------------------

# Summary

This R Markdown file demonstrates: - How to structure commits in a Git
project  
- How to use branches for testing  
- How to document your workflow in a GitHub-ready format
