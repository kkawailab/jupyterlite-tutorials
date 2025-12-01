# JupyterLite Tutorials

## 概要
このリポジトリには JupyterLite で配信するインタラクティブな Notebook チュートリアルがまとまっています。`pandas`/`matplotlib` などの基礎から、Folium や Statsmodels を使った可視化・分析手法を、ブラウザだけで再現できる構成です。仕組みやコントリビュートの詳細は `AGENTS.md` も参照してください。

## コンテンツ構成
- `jupyterlite_beginner_tutorial_with_exercises_v2.ipynb` — JupyterLite の基本操作と演習問題。
- `pandas_jupyterlite_tutorial.ipynb` — DataFrame の整形と集約テクニック。
- `matplotlib_jupyterlite_tutorial.ipynb` — グラフ描画の基本とカスタマイズ。
- `leaflet_folium_jupyterlite_tutorial.ipynb` — Folium/Leaflet による地図表示（名古屋市立大学経済学部を中心としたサンプル）。
- `leaflet_folium_jupyterlite_tutorial_tokai.ipynb` — Folium/Leaflet の発展編（東海4県の GeoJSON 表示）。
- `statsmodels_jupyterlite_tutorial_v2.ipynb` — 回帰分析と統計モデリングの実践。

Notebook 以外のデータや画像を追加する場合は Notebook 名と同じプリフィックスのサブディレクトリを作成し、トップレベルを整理します。

## エンドユーザ向け：チュートリアルの使い方

### 収録コンテンツ

| ファイル | 内容 |
|---------|------|
| `jupyterlite_beginner_tutorial_with_exercises_v2.ipynb` | JupyterLite の基本操作と演習問題 |
| `pandas_jupyterlite_tutorial.ipynb` | DataFrame の整形と集約テクニック |
| `matplotlib_jupyterlite_tutorial.ipynb` | グラフ描画の基本とカスタマイズ |
| `leaflet_folium_jupyterlite_tutorial.ipynb` | Folium/Leaflet による地図表示 |
| `leaflet_folium_jupyterlite_tutorial_tokai.ipynb` | Folium/Leaflet 発展編（東海4県 GeoJSON） |
| `statsmodels_jupyterlite_tutorial_v2.ipynb` | 回帰分析と統計モデリング |

### 利用方法

1. **ブラウザから直接利用**：JupyterLite でホストされている場合、ブラウザで URL にアクセスするだけで、インストール不要で Notebook を実行できます

2. **ローカルで利用する場合**：
   ```bash
   # 仮想環境を作成
   python -m venv .venv && source .venv/bin/activate

   # JupyterLab をインストール
   pip install -U jupyterlab

   # Notebook を開く
   jupyter lab <ファイル名>.ipynb
   ```

3. **学習の進め方**：
   - 初心者は `jupyterlite_beginner_tutorial_with_exercises_v2.ipynb` から始めることをお勧めします
   - 各 Notebook にはセルごとに実行できるコード例と演習問題が含まれています
   - Shift + Enter でセルを実行しながら進めてください

## 開発者向け：編集とビルド

1. Python 3.10 以上を用意し、仮想環境を作成:
   ```bash
   python -m venv .venv && source .venv/bin/activate
   ```
2. 執筆やローカル検証に必要なツールを導入:
   ```bash
   pip install -U jupyterlab jupyterlite nbconvert
   ```
3. Notebook を編集する場合は `jupyter lab pandas_jupyterlite_tutorial.ipynb` のように開いて作業します。
4. 変更内容をブラウザ配信向けにまとめるには `jupyter lite build` を実行し、生成物 (`_output/` 配下) をホストへ配置します。
5. すべての Notebook が問題なく動くか確認するには `jupyter nbconvert --execute --inplace <notebook>.ipynb` を利用してください。ランダム性のあるセルではシードを固定します。

## 更新履歴
- 2025-11-21: 初版公開。各種 JupyterLite チュートリアルと `AGENTS.md` を追加。
  - 重複ファイル `leaflet_folium_jupyterlite_tutorial (1).ipynb` を削除。
  - `leaflet_folium_jupyterlite_tutorial.ipynb` のサンプル座標を浜松市から名古屋市立大学経済学部（滝子キャンパス）に変更。
  - 各ファイルの緯度経度の記述ミスを修正。
  - `leaflet_folium_jupyterlite_tutorial_tokai.ipynb` を追加（東海4県の GeoJSON 表示の発展編）。
