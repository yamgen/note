# Python開発の第一歩

## 前提

### 環境およびバージョン
- Windows 10、Windows 11
- Python 3.10 以降
- Visual Studio Code 1.71

### Pythonのセットアップ

#### Pythonのインストール
- [Pythonの公式サイト](https://www.python.org/)からバージョン3.XXインストーラーをダウンロードしてインストールする。
- インストール時に「Add Python 3.x to PATH」にチェックを入れる。
- `py -3.XX --version`でバージョンが表示されることを確認する。

#### WindowsにおけるPython
- Windows10以降、標準でPythonがインストールされている。
- ただしMicrosoft Storeを開くダミーコマンドであるためPythonプログラムの実行はできない

```
python --version
# バージョンが表示されない
```

### pythonの基本コマンド

#### pyコマンド
- pyコマンドはPythonのバージョンを切り替えるためのコマンドである。
- Windowsでは複数のpythonをインストール後にpyコマンドを用いて任意のバージョンを指定して実行することができる。
- 実行は`py -3.XX`で行う。

例）Python3.10を実行する場合
```
# バージョン確認
> py -3.10 --version
Python 3.10.6

# pipのバージョン確認
> py -3.10 -m pip --version
```

#### pipコマンド
- pipはPythonのパッケージ管理ツールである。
- pipコマンドを用いてpypi(Python Package Index)からサードパーティパッケージをインストールすることができる。

例）requestsパッケージをインストールする場合
```
> py -3.10 -m pip install requests
```

#### venvコマンド
- venvはPythonの仮想環境を作成するためのコマンドである。
- 仮想環境を作成することで、プロジェクトごとにパッケージ、pythonランタイムのバージョンを管理することができる。
- 仮想環境を作成すると、プロジェクトフォルダにvenvフォルダが作成される。

例）venvを作成する場合
```
> py -3.10 -m venv .venv
```

#### 仮想環境の有効化
- 