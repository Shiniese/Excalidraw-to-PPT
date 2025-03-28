# **Excalidraw-to-PPT**

![Python](https://img.shields.io/badge/python-3.12-blue) ![License](https://img.shields.io/badge/license-MIT-green)

`.excalidraw` ファイルを PowerPoint プレゼンテーション (PPT) に自動的に変換する Python ツールです。`.excalidraw` ファイルから埋め込まれた画像を抽出し、PNG 形式で保存し、整然と整理された形式でパワーポイントスライドにまとめます。

---

## **機能**
- 自動的に `.excalidraw` ファイルから base64 エンコードされた画像を抽出します。
- 抽出した画像を専用フォルダ内に個別の PNG ファイルとして保存します。
- 抽出されたすべての画像をグリッドレイアウトで配置したパワーポイントプレゼンテーションを生成します。
- 単一ディレクトリに複数の `.excalidraw` ファイルを処理可能です。

---

## **インストール方法**

1. **リポジトリをクローンする**
   ```bash
   git clone https://github.com/Shiniese/Excalidraw-to-PPT.git
   cd Excalidraw-to-PPT
   ```

2. **依存関係のインストール**
   必要な Python ライブラリを `pip` を使用してインストールします:
   ```bash
   pip install python-pptx Pillow
   ```

3. **Excalidraw ファイルをセットする**
   プロジェクトディレクトリに `.excalidraw` ファイルをコピーします。

---

## **使い方**

1. スクリプトを実行します：
   ```bash
   python excalidraw_to_ppt.py
   ```

2. このツールは以下のことを行います：
   - 現在のディレクトリにあるすべての `.excalidraw` ファイルから画像を抽出します。
   - 画像を各ファイル名に対応したサブフォルダに保存します。
   - 抽出された画像が整頓されて配置されたパワーポイントファイル（`excalidraw_to_ppt.pptx`）を生成します。

---

## **例**

#### 入力:
次の三つの `.excalidraw` ファイルがあるとします：
- `diagram1.excalidraw`
- `diagram2.excalidraw`
- `notes.excalidraw`

#### 出力:
- `diagram1/` フォルダに抽出された画像（例：`diagram1-1.png`, `diagram1-2.png` など）。
- `diagram2/` フォルダに抽出された画像（例：`diagram2-1.png`, `diagram2-2.png` など）。
- `notes/` フォルダに抽出された画像（例：`notes-1.png` など）。

そして、対応する画像が整然と配置されたスライドを持つパワーポイントファイル (`excalidraw_to_ppt.pptx`) が出力されます。

---

## **依存関係**

以下の Python ライブラリが必要です：
- `python-pptx` （パワーポイントプレゼンテーション作成）
- `Pillow` （画像処理）
- `os`, `json`（標準的な Python モジュール）

それらを以下のコマンドを使用してインストールしてください：
```bash
pip install python-pptx Pillow
```

---

## **貢献方法**

本プロジェクトに貢献したい場合：
1. リポジトリをフォークします。
2. 新しいブランチを作ります（例：`git checkout -b feature/YourFeatureName`）。
3. 変更をコミットします（例：`git commit -m "Add some feature"`）。
4. ブランチをプッシュします（例：`git push origin feature/YourFeatureName`）。
5. プルリクエストを作成します。

---

## **ライセンス**

このプロジェクトは **MIT ライセンス** の下で配布されています。詳細を見るには [LICENSE](https://github.com/Shiniese/Excalidraw-to-PPT/blob/main/LICENSE) ファイルをご確認ください。

---

## **クレジット**

- デザインタスクとプレゼンテーション間のワークフローを自動化する必要性にインスピレーションを受けました。
- Python ライブラリ `python-pptx` と `Pillow` によって提供されました。
