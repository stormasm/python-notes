
### Steps to get started

- Assuming you have uv installed
- Go to *tmp34* or where ever you want the root of your project to be

```rust
uv init piet
cd piet
uv add --dev ipykernel

uv run ipython kernel install --user --env VIRTUAL_ENV $(pwd)/.venv --name=project
Installed kernelspec project in /Users/ma/Library/Jupyter/kernels/project

uv run --with jupyter jupyter lab
```

### References

- [how to install uv](https://docs.astral.sh/uv/configuration/installer/#disabling-shell-modifications)
- [using uv with jupyter](https://docs.astral.sh/uv/guides/integration/jupyter/)
