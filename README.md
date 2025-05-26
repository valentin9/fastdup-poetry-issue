Reproduce the issue:
1. install python 3.11
2. install latest poetry (e.g. `pip install poetry`)
3. run `poetry install`
4. check the output of `poetry show fastdup --tree`

The current output:
```
fastdup 2.23 Fast tool for gaining insights from large image repositories.
├── certifi *
└── sentry-sdk *
    ├── certifi * 
    └── urllib3 >=1.26.11
```
