## Test Package

```bash
pipenv install pip setuptools wheel tqdm twine
chmod +x kokoko
pipenv run python setup.py sdist bdist_wheel
pipenv run python -m twine upload dist/*
```

## Local

```bash
pipenv install
pipenv run pip install dist/kokoko-0.2-py3-none-any.whl
```

## Remote

```bash
pipenv install kokoko
pipenv run kokoko
```

## Uninstall

```bash
pipenv uninstall kokoko
```