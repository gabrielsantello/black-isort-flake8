```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ poetry run flake8 main.py
main.py:7:1: E302 expected 2 blank lines, found 1
main.py:26:77: W291 trailing whitespace
main.py:27:80: E501 line too long (89 > 79 characters)
main.py:58:80: E501 line too long (154 > 79 characters)
main.py:66:1: E305 expected 2 blank lines after class or function definition, found 1
main.py:72:53: W292 no newline at end of file
```
```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ poetry add black
Using version ^24.2.0 for black

Updating dependencies
Resolving dependencies... (0.7s)

Package operations: 7 installs, 0 updates, 0 removals

  • Installing colorama (0.4.6)
  • Installing click (8.1.7)
  • Installing mypy-extensions (1.0.0)
  • Installing packaging (23.2)
  • Installing pathspec (0.12.1)
  • Installing platformdirs (4.2.0)
  • Installing black (24.2.0)

Writing lock file
```
```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ poetry run black main.py
reformatted main.py

All done! ✨ 🍰 ✨
1 file reformatted.
```
```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ poetry run flake8 main.py
main.py:27:77: W291 trailing whitespace
main.py:28:80: E501 line too long (89 > 79 characters)
```
```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ touch .flake8
```
```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ poetry run flake8 main.py
main.py:27:77: W291 trailing whitespace
```
```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ poetry run flake8 main.py
```
```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ poetry run black  main.py
All done! ✨ 🍰 ✨
1 file left unchanged.
```
```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ poetry add isort
Using version ^5.13.2 for isort

Updating dependencies
Resolving dependencies... (0.1s)

Package operations: 1 install, 0 updates, 0 removals

  • Installing isort (5.13.2)

Writing lock file
```
```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ poetry run isort main.py
Fixing C:\Users\gvsan\Documents\bootcamp\data-engineering-roadmap\black-isort-flake8\main.py
```
```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ poetry run task format
```
```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ poetry run pre-commit install
pre-commit installed at .git\hooks\pre-commit
```
```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ git add .pre-commit-config.yaml
```
```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ git commit -m 'pre-commit sample'
[WARNING] Unstaged files detected.
[INFO] Stashing unstaged files to C:\Users\gvsan\.cache\pre-commit\patch1709069735-16816.
[INFO] Initializing environment for https://github.com/pre-commit/pre-commit-hooks.
[INFO] Initializing environment for https://github.com/psf/black-pre-commit-mirror.
[INFO] Initializing environment for https://github.com/pycqa/isort.
[INFO] Initializing environment for https://github.com/pycqa/flake8.
[INFO] Installing environment for https://github.com/pre-commit/pre-commit-hooks.
[INFO] Once installed this environment will be reused.
[INFO] This may take a few minutes...
[INFO] Installing environment for https://github.com/psf/black-pre-commit-mirror.
[INFO] Once installed this environment will be reused.
[INFO] This may take a few minutes...
[INFO] Installing environment for https://github.com/pycqa/isort.
[INFO] Once installed this environment will be reused.
[INFO] This may take a few minutes...
[INFO] Installing environment for https://github.com/pycqa/flake8.
[INFO] Once installed this environment will be reused.
[INFO] This may take a few minutes...
trim trailing whitespace.............................(no files to check)Skipped
fix end of files.....................................(no files to check)Skipped
check yaml...........................................(no files to check)Skipped
check toml...........................................(no files to check)Skipped
detect private key...................................(no files to check)Skipped
check for added large files..........................(no files to check)Skipped
black................................................(no files to check)Skipped
isort (python).......................................(no files to check)Skipped
flake8...............................................(no files to check)Skipped
[INFO] Restored changes from C:\Users\gvsan\.cache\pre-commit\patch1709069735-16816.
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   terminal.md

no changes added to commit (use "git add" and/or "git commit -a")
```
```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ git commit -m 'pre-commit sample'
[WARNING] Unstaged files detected.
[INFO] Stashing unstaged files to C:\Users\gvsan\.cache\pre-commit\patch1709069735-16816.
[INFO] Initializing environment for https://github.com/pre-commit/pre-commit-hooks.
[INFO] Initializing environment for https://github.com/psf/black-pre-commit-mirror.
[INFO] Initializing environment for https://github.com/pycqa/isort.
[INFO] Initializing environment for https://github.com/pycqa/flake8.
[INFO] Installing environment for https://github.com/pre-commit/pre-commit-hooks.
[INFO] Once installed this environment will be reused.
[INFO] This may take a few minutes...
[INFO] Installing environment for https://github.com/psf/black-pre-commit-mirror.
[INFO] Once installed this environment will be reused.
[INFO] This may take a few minutes...
[INFO] Installing environment for https://github.com/pycqa/isort.
[INFO] Once installed this environment will be reused.
[INFO] This may take a few minutes...
[INFO] Installing environment for https://github.com/pycqa/flake8.
[INFO] Once installed this environment will be reused.
[INFO] This may take a few minutes...
trim trailing whitespace.............................(no files to check)Skipped
fix end of files.....................................(no files to check)Skipped
check yaml...........................................(no files to check)Skipped
check toml...........................................(no files to check)Skipped
detect private key...................................(no files to check)Skipped
check for added large files..........................(no files to check)Skipped
black................................................(no files to check)Skipped
isort (python).......................................(no files to check)Skipped
flake8...............................................(no files to check)Skipped
[INFO] Restored changes from C:\Users\gvsan\.cache\pre-commit\patch1709069735-16816.
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   terminal.md

no changes added to commit (use "git add" and/or "git commit -a")
```
```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   terminal.md

no changes added to commit (use "git add" and/or "git commit -a")
```
```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ git add .
```
```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ git commit -m 'terminal'
trim trailing whitespace.................................................Passed
fix end of files.........................................................Failed
- hook id: end-of-file-fixer
- exit code: 1
- files were modified by this hook

Fixing terminal.md

check yaml...........................................(no files to check)Skipped
check toml...........................................(no files to check)Skipped
detect private key.......................................................Passed
check for added large files..............................................Passed
black................................................(no files to check)Skipped
isort (python).......................................(no files to check)Skipped
flake8...............................................(no files to check)Skipped
```
```
gvsan@Gabriel MINGW64 ~/Documents/bootcamp/data-engineering-roadmap/black-isort-flake8 (main)
$ git push
Everything up-to-date
```
