# pythonのvscode remote container開発環境調整用レポジトリ

## 概要

- dotfileサポート
- 保存時に自動で色々実行(mypy, flake8, black, isort)
  - mypy...型チェック
  - flake8...スタイル、エラー、複雑度チェックなどができるリンター
  - black...pythonの標準ライブラリに含まれているコーディング規約であるPEP8をもとに独自のルールを追加したフォーマッター
  - importを名前順に並び替える
- テストツールはpytest

## メモ

### testsディレクトリの__init__.pyなに

- これがないと、うまくテストファイルがうまく認識されない
- [vscode公式](https://code.visualstudio.com/docs/python/testing#_test-discovery)にそうしろって書いててできた
- `__init__.py`がpythonにとって特別な意味を持ったファイルのよう
