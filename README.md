# 環境構築
## WSL(1.2.5.0)
vscodeに以下の拡張機能をインストールする  
* WSL  
* SQLite
* Python

左下の<font color="Blue">><</font>からwslに接続を行う  
Ctrl + @ でターミナルを起動  
適当なフォルダを作成し，リポジトリをクローンする  
`git clone https://github.com/Tanakaryuki/FastAPI_APP.git`  

フォルダに移動する  
`cd FastAPI_APP`  

仮想環境の作成  
`python -m venv env`  

(仮想環境の作成に失敗した場合)  
`sudo apt install python3-venv`  

仮想環境を有効化  
`. env/bin/activate`  

ライブラリをインストール  
`pip install -r requierment.txt`  

(ライブラリのインストールに失敗した場合)  
`sudo apt install python3-pip`  

<br>

# 開発の開始  
FastAPIの起動  
`uvicorn main:app --reload`  

ブラウザで[http://localhost:8000](http://localhost:8000)を開く  

<br>

# デバッグについて  
SQLiteの閲覧  
vscode上で  
`Ctrl + Shift + p`  
`SQLite: Open Database`  

APIのテスト  
[http://localhost:8000/docs](http://localhost:8000/docs)から行う  

APIドキュメントの確認  
[http://localhost:8000/redoc](http://localhost:8000/redoc)から行う  

<br>

# 開発の終了  
FastAPIの停止  
`Ctrl + c`  

仮想環境の無効化  
`deactivate`  
