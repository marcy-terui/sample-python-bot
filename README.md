Sample Slack Bot Project
=========

## Description
Slack Botのプロジェクトサンプルリポジトリ

## Requirements
- Python 3.5.3
- pip
- virtualenv

## Setup

```
virtualenv .venv
pip install -r requirements.txt
```

## Usage
T.B.D

## Modules

```
.

├── http.py    # HTTP Server起動スクリプト
├── slack.py   # Slack Bot起動スクリプト
└── pybot
    ├── http   # HTTP処理（Controller）
    ├── slack  # Slack Bot Plugins (Handler)
    ├── config # 設定ファイル
    └── libs   # 共通処理
```
