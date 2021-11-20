# pythonのvscode remote container開発環境調整用レポジトリ

## メモ

### testsディレクトリの__init__.pyなに

- これがないと、うまくテストファイルがうまく認識されない
- [vscode公式](https://code.visualstudio.com/docs/python/testing#_test-discovery)にそうしろって書いててできた
- `__init__.py`がpythonにとって特別な意味を持ったファイルのよう
