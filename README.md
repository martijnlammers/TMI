## Setup docs
### Prerequisits
* [Python 3.12.6](https://www.python.org/downloads/)

### MkDocs setup
1. Create a virtual Python environment.
```bash
# In root of repository
python -m venv venv
```
2. [Activate virtual environment.](https://docs.python.org/3/library/venv.html#how-venvs-work) 
3. Install the dependencies for mkdocs material.
```bash
pip install mkdocs-material
```

### Hosting 
Start a local server for live reloading when applying changes to the documentation.
```bash
mkdocs serve
```
The documentation should be accessible by browsing to http://127.0.0.1:8000/.

### Updating documentation
The docs branch is protected. No direct commits can be pushed to it. Alike the main branch,
the changes must go through a PR. Changes to this branch automatically trigger 
GitHub actions, which is responsible for deployment of the updated documentation.

### References
* [Markdown Syntax](https://www.markdownguide.org/basic-syntax/)
* [MkDocs Material](https://squidfunk.github.io/mkdocs-material/)