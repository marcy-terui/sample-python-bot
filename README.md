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
    ├── http   # HTTP処理 (Controller)
    ├── slack  # Slack Bot Plugins (Handler)
    ├── config # 設定ファイル
    └── libs   # 共通処理
```

### Points
- rootに置くのは起動スクリプトのみ。それ以外の実処理は種類別でディレクトリを分ける
  - rootを雑多にしない
  - 起動スクリプトもscriptsのようなディレクトリで分けてもしまっても良い
  - 起動スクリプトは必要なmoduleをimportして起動するだけ。ここには処理を書かない。
- 実処理には固有のModule名を付けて、外部ライブラリと明確に区別する（この例では `pybot` ）
- `http` の `Controller` や `slack` の `Handler` も単純な処理の振り分けに専念して実処理はさらに `libs` 内で分割していくと尚良
