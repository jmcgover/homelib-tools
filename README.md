# homelib
Tools for cataloguing a home media library.

## Libraries Used
- [`isbntools`](https://pypi.org/project/isbntools/)

## Development

Initialize `venv`:
```bash
python3 -m venv venv && source venv/bin/activate
```

Install tools:
```bash
pip install -U pip pip-tools
```

Pin requirements files:
```bash
pip-compile -o requirements.txt pyproject.toml
```
```bash
pip-compile --extra dev -o requirements-dev.txt pyproject.toml
```

Sync to requirements files:
```bash
pip-sync requirements*.txt
```
