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
