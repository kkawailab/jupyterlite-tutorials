# JupyterLite Tutorials

## 概要
このリポジトリには JupyterLite で配信するインタラクティブな Notebook チュートリアルがまとまっています。`pandas`/`matplotlib` などの基礎から、Folium や Statsmodels を使った可視化・分析手法を、ブラウザだけで再現できる構成です。仕組みやコントリビュートの詳細は `AGENTS.md` も参照してください。

## コンテンツ構成
- `jupyterlite_beginner_tutorial_with_exercises_v2.ipynb` — JupyterLite の基本操作と演習問題。
- `pandas_jupyterlite_tutorial.ipynb` — DataFrame の整形と集約テクニック。
- `matplotlib_jupyterlite_tutorial.ipynb` — グラフ描画の基本とカスタマイズ。
- `leaflet_folium_jupyterlite_tutorial.ipynb` および `leaflet_folium_jupyterlite_tutorial (1).ipynb` — Folium/Leaflet による地図表示のバリエーション。
- `statsmodels_jupyterlite_tutorial_v2.ipynb` — 回帰分析と統計モデリングの実践。

Notebook 以外のデータや画像を追加する場合は Notebook 名と同じプリフィックスのサブディレクトリを作成し、トップレベルを整理します。

## 使い方
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
