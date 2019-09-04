## Test Package

```bash
pipenv install pip setuptools whell tqdm twine
chmod +x kokoko
pipenv run python setup.py sdist bdist_wheel
pipenv run python -m twine upload dist/*
```

## Check

```bash
pipenv run pip install dist/kokoko-0.2-py3-none-any.whl
pipenv run pip install kokoko
pipenv run kokoko
```