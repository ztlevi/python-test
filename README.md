# Test

Test mspyls. Put something like this below in your `.bashrc/.zshrc`.

```sh
export PYTHONPATH=$PYTHONPATH:{dir}/python-test/python_root
```

Make sure your emacs can get proper `PYTHONPATH` env with `(getenv "PYTHONPATH")`

# Issue

mspyls cannot resolve symlink modules. Reproduce the issue by navigating to `{project_root}/test`, put your cursor under `test_func` and trigger `M-x lsp-ui-peek-find-definitions`.
