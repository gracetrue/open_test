# Teacher-student Dialogue System for Intervention in Children using GLM

## Development Environment(Requirements)

- Ubuntu 20.04 LTS
- python 3.11.14 
- SQLite3 3.31.1
- numpy 2.3.5
- pandas 2.3.3
- transformers 4.57.6
- openpyxl 3.1.5 
- flask 3.1.2
- PyTorch:
    - torch==2.7.0+cu118
    - torchvision==0.22.0+cu118
    - torchaudio==2.7.0+cu118

## Installation

0) Database managing을 위한 sqlite3 installation

```bash
~$ sudo apt update
~$ sudo apt install -y sqlite3
```

1) Create and activate virtual environment

```bash
~$ python -m venv .venv
~$ source .venv/bin/activate
```

2) Install Bootstrap tools

```bash
(.venv)~$ python -m pip install -U pip setuptools wheel pip-tools
```

3) Install dependencies

```bash
(.venv)~$ python -m pip install torch==2.7.0 torchvision==0.22.0 torchaudio==2.7.0 --index-url https://download.pytorch.org/whl/cu118
(.venv)~$ python -m pip install -r requirements.txt
```

4) API server 켜기 

```bash
(.venv)~$ cd api_server
(.venv)~/api_server$ python app.py
```

5) RUN: server test shell script

```bash
(.venv)~$ cd api_server
(.venv)~$ ./test_api.sh
```