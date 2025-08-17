# python-docker-template

DevContainerでPythonの開発環境を作るためのテンプレート

Pythonのパッケージ管理にはpoetryを使用

※ [Poetryの公式ドキュメント](https://python-poetry.org/docs/configuration#virtualenvscreate) では仮想環境の作成が推奨されているため、このテンプレートでもDockerコンテナ内で仮想環境を作成し、依存関係を分離する

## Extensions

以下の拡張機能が自動でインストールされる

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

1. [Docker Hub](https://hub.docker.com/_/python/) からPythonのタグ（バージョン）を選択
2. 選択したタグを `Dockerfile` に記入
3. VSCodeで `Reopen in Container` を実行（DevContainer環境を起動）
4. コンテナ内で `poetry init` を実行し、プロジェクトをセットアップ
5. 必要なパッケージを `poetry add <package-name>` で追加
