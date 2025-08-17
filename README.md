# python-docker-template

DevContainerでPythonの開発環境を作るためのテンプレートです。

Pythonのパッケージ管理にはpoetryを使用します。

※ [Poetryの公式ドキュメント](https://python-poetry.org/docs/configuration#virtualenvscreate) では、Dockerを利用する場合でも仮想環境を作成することが推奨されているため、このテンプレートでもDockerコンテナ内で仮想環境を作成して依存関係を分離します。

## Extensions

以下のVSCode拡張機能が自動でインストールされます。

- GitHub Copilot (`GitHub.copilot`)
- GitHub Copilot Chat (`GitHub.copilot-chat`)
- Git Graph (`mhutchie.git-graph`)
- GitLens (`eamodio.gitlens`)
- Python (`ms-python.python`)
- Jupyter (`ms-toolsai.jupyter`)
- Ruff (`charliermarsh.ruff`)
- Mypy Type Checker (`ms-python.mypy-type-checker`)
- AutoDocstring (`njpwerner.autodocstring`)
- Path Intellisense (`christian-kohler.path-intellisense`)
- Gutter Preview (`kisstkondoros.vscode-gutter-preview`)
- Rainbow CSV (`mechatroner.rainbow-csv`)

## Usage

1. [Docker Hub](https://hub.docker.com/_/python/) から任意のPythonのタグ（バージョン）を選択する
2. 選択したタグを `Dockerfile` に記入する
3. VSCodeで `Reopen in Container` を実行する
4. コンテナ内で `poetry init` を実行し、プロジェクトをセットアップする
5. 必要なパッケージを `poetry add <package-name>` で追加する
