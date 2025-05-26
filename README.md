Reproduce the issue:
1. install python 3.11
2. install latest poetry (e.g. `pip install poetry`)
3. run `poetry install`
4. check the output of `poetry show fastdup --tree`

output:
```commandline
fastdup 2.23 Fast tool for gaining insights from large image repositories.
├── certifi *
└── sentry-sdk *
    ├── certifi * 
    └── urllib3 >=1.26.11
```

And with fastdup 2.22:
1. change fastdup version by running `poetry add "fastdup@2.22"`
2. run `poetry show fastdup --tree`

output: 
```commandline
fastdup 2.22 Fast tool for gaining insights from large image repositories.
├── aiofiles >=24.1.0,<24.2.0
├── certifi *
├── cryptography 44.0.1
│   └── cffi >=1.12 
│       └── pycparser * 
├── duckdb 1.2.0
├── duckdb-engine >=0.13.0,<0.14.0
│   ├── duckdb >=0.5.0 
│   ├── packaging >=21 
│   └── sqlalchemy >=1.3.22 
│       ├── greenlet >=1 
│       └── typing-extensions >=4.6.0 
├── fastapi 0.115.8
│   ├── pydantic >=1.7.4,<1.8 || >1.8,<1.8.1 || >1.8.1,<2.0.0 || >2.0.0,<2.0.1 || >2.0.1,<2.1.0 || >2.1.0,<3.0.0 
│   │   ├── annotated-types >=0.6.0 
│   │   ├── pydantic-core 2.33.2 
│   │   │   └── typing-extensions >=4.6.0,<4.7.0 || >4.7.0 
│   │   ├── typing-extensions >=4.12.2 (circular dependency aborted here)
│   │   └── typing-inspection >=0.4.0 
│   │       └── typing-extensions >=4.12.0 (circular dependency aborted here)
│   ├── starlette >=0.40.0,<0.46.0 
│   │   └── anyio >=3.4.0,<5 
│   │       ├── idna >=2.8 
│   │       ├── sniffio >=1.1 
│   │       └── typing-extensions >=4.5 (circular dependency aborted here)
│   └── typing-extensions >=4.8.0 (circular dependency aborted here)
├── google-auth 2.29.0
│   ├── cachetools >=2.0.0,<6.0 
│   ├── pyasn1-modules >=0.2.1 
│   │   └── pyasn1 >=0.6.1,<0.7.0 
│   └── rsa >=3.1.4,<5 
│       └── pyasn1 >=0.1.3 (circular dependency aborted here)
├── httpx 0.26.0
│   ├── anyio * 
│   │   ├── idna >=2.8 
│   │   ├── sniffio >=1.1 
│   │   └── typing-extensions >=4.5 
│   ├── certifi * 
│   ├── httpcore ==1.* 
│   │   ├── certifi * (circular dependency aborted here)
│   │   └── h11 >=0.16 
│   ├── idna * (circular dependency aborted here)
│   └── sniffio * (circular dependency aborted here)
├── jinja2 3.1.5
│   └── markupsafe >=2.0 
├── joblib >=1.2.0,<1.3.0
├── jsonschema 4.22.0
│   ├── attrs >=22.2.0 
│   ├── jsonschema-specifications >=2023.03.6 
│   │   └── referencing >=0.31.0 
│   │       ├── attrs >=22.2.0 (circular dependency aborted here)
│   │       ├── rpds-py >=0.7.0 
│   │       └── typing-extensions >=4.4.0 
│   ├── referencing >=0.28.4 (circular dependency aborted here)
│   └── rpds-py >=0.7.1 (circular dependency aborted here)
├── nest-asyncio *
├── numpy >1.23.0
├── opencv-python-headless >=4.8.0.0
│   └── numpy >=1.23.5 
├── packaging *
├── pandas >=2.0.3
│   ├── numpy >=1.23.2 
│   ├── python-dateutil >=2.8.2 
│   │   └── six >=1.5 
│   ├── pytz >=2020.1 
│   └── tzdata >=2022.7 
├── pillow 10.3.0
├── pillow-heif *
│   └── pillow >=10.1.0 
├── polars 0.20.0
├── psutil *
├── pyarrow 14.0.1
│   └── numpy >=1.16.6 
├── pydantic *
│   ├── annotated-types >=0.6.0 
│   ├── pydantic-core 2.33.2 
│   │   └── typing-extensions >=4.6.0,<4.7.0 || >4.7.0 
│   ├── typing-extensions >=4.12.2 (circular dependency aborted here)
│   └── typing-inspection >=0.4.0 
│       └── typing-extensions >=4.12.0 (circular dependency aborted here)
├── pyjwt 2.8.0
├── pyopenssl >=24.0.0
│   ├── cryptography >=41.0.5,<46 
│   │   └── cffi >=1.12 
│   │       └── pycparser * 
│   └── typing-extensions >=4.9 
├── python-multipart >0.0.18
├── pyyaml >=6.0,<7.0
├── requests >=2.31.0
│   ├── certifi >=2017.4.17 
│   ├── charset-normalizer >=2,<4 
│   ├── idna >=2.5,<4 
│   └── urllib3 >=1.21.1,<3 
├── scikit-learn 1.5.0
│   ├── joblib >=1.2.0 
│   ├── numpy >=1.19.5 
│   ├── scipy >=1.6.0 
│   │   └── numpy >=1.23.5,<2.5 (circular dependency aborted here)
│   └── threadpoolctl >=3.1.0 
├── sentry-sdk 2.27.0
│   ├── certifi * 
│   └── urllib3 >=1.26.11 
├── setproctitle 1.3.3
├── setuptools 72.2.0
├── sqlalchemy >=2.0.29,<2.1.0
│   ├── greenlet >=1 
│   └── typing-extensions >=4.6.0 
├── starlette 0.40.0
│   └── anyio >=3.4.0,<5 
│       ├── idna >=2.8 
│       ├── sniffio >=1.1 
│       └── typing-extensions >=4.5 
├── starlette-prometheus 0.9.0
│   ├── prometheus-client >=0.12,<0.13 
│   └── starlette >=0.12.2 
│       └── anyio >=3.4.0,<5 
│           ├── idna >=2.8 
│           ├── sniffio >=1.1 
│           └── typing-extensions >=4.5 
├── tqdm 4.66.3
│   └── colorama * 
└── uvicorn 0.29.0
    ├── click >=7.0 
    │   └── colorama * 
    └── h11 >=0.8 
```
