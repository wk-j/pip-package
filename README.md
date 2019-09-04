## Test

```bash
pipenv install pip setuptools wheel tqdm twine
chmod +x kokoko
pipenv run python setup.py sdist bdist_wheel
pipenv run python -m twine upload dist/*
```

## Local

```bash
pipenv run pip install dist/kokoko-0.3-py3-none-any.whl
pipenv run pip uninstall dist/kokoko-0.3-py3-none-any.whl
```

## Remote

```bash
pipenv install kokoko
pipenv run kokoko
pipenv uninstall kokoko
```

## Check

```bash
pipenv run python check/p.py
```