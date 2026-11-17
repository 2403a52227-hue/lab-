# GitHub Actions Automated Testing Demo

This starter project runs Python tests automatically whenever code is pushed to
`main` or `master`, and when a pull request targets either branch.

## Files

- `.github/workflows/test.yml` — GitHub Actions workflow
- `test_calculator.py` — sample pytest test cases
- `requirements.txt` — test dependency

## Run locally

```bash
python -m pip install -r requirements.txt
python -m pytest -v
```

## Upload to GitHub

1. Create a new GitHub repository.
2. Extract this ZIP file.
3. Upload the contents of the `github-actions-testing` folder to the repository
   (make sure `.github/workflows/test.yml` is included).
4. Commit the files to the `main` branch.
5. Open the repository's **Actions** tab to see the workflow run.

You can also push the folder using Git from VS Code:

```bash
git init
git add .
git commit -m "Add automated tests and GitHub Actions workflow"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```

Replace the remote URL with your own repository URL.
