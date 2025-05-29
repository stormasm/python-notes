
### Where is stuff located

The uv binaries are located here

```rust
/Users/ma/mia/uv/bin
```

Python is located here:

```rust
/Users/ma/mia/uv
```

### Installing uv

```rust
curl -LsSf https://astral.sh/uv/install.sh | env UV_INSTALL_DIR="/Users/ma/mia/uv/bin" sh
```

### Installing Python

```rust
uv python install -i "/Users/ma/mia/uv"
```

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

- [how to install uv](https://docs.astral.sh/uv/configuration/installer)
- [how to uninstall uv](https://docs.astral.sh/uv/getting-started/installation/#uninstallation)
- [how to install python](https://docs.astral.sh/uv/reference/cli/#uv-python)
- [using uv with jupyter](https://docs.astral.sh/uv/guides/integration/jupyter/)
