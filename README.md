# pre-commit js-beautify
For pre-commit: see https://github.com/pre-commit/pre-commit

For js-beautify: see https://github.com/emilkholod/js-beautify-guidelines


### Using js-beautify with pre-commit

Add this to your `.pre-commit-config.yaml`:
```yaml
    -   repo: https://github.com/emilkholod/js-beautify-guidelines.git
        sha: ''  # Use the sha you want to point at
        hooks:
        -   id: js-beautify
        args: [
            '--type=html',
            '--replace',
            '--end-with-newline',
            '--indent-size=4',
            '--indent-char= ',
            '--max-preserve-newlines=10',
            '--preserve-newlines=true',
            '--wrap-attributes=force-aligned',
            '--wrap-line-length=120',
            '--indent-empty-lines=false',
            '--brace-style=collapse',
            '--indent-scripts=normal'
        ]
```
