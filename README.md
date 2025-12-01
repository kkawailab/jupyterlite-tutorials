# JupyterLite Tutorials

## 概要
このリポジトリには JupyterLite で配信するインタラクティブな Notebook チュートリアルがまとまっています。`pandas`/`matplotlib` などの基礎から、Folium や Statsmodels を使った可視化・分析手法を、ブラウザだけで再現できる構成です。仕組みやコントリビュートの詳細は `AGENTS.md` も参照してください。

## コンテンツ構成
- [`jupyterlite_beginner_tutorial_with_exercises_v2.ipynb`](./jupyterlite_beginner_tutorial_with_exercises_v2.ipynb) — JupyterLite の基本操作と演習問題。
- [`pandas_beginner_tutorial.ipynb`](./pandas_beginner_tutorial.ipynb) — pandas 初級：Series/DataFrame の基本、選択、フィルタリング、統計量。
- [`pandas_intermediate_tutorial.ipynb`](./pandas_intermediate_tutorial.ipynb) — pandas 中級：groupby、欠損値処理、結合、時系列、文字列操作。
- [`pandas_jupyterlite_tutorial.ipynb`](./pandas_jupyterlite_tutorial.ipynb) — DataFrame の整形と集約テクニック。
- [`matplotlib_beginner_tutorial.ipynb`](./matplotlib_beginner_tutorial.ipynb) — matplotlib 初級：折れ線、散布図、棒グラフ、ヒストグラム、円グラフ。
- [`matplotlib_intermediate_tutorial.ipynb`](./matplotlib_intermediate_tutorial.ipynb) — matplotlib 中級：サブプロット、軸設定、注釈、seaborn連携。
- [`matplotlib_jupyterlite_tutorial.ipynb`](./matplotlib_jupyterlite_tutorial.ipynb) — グラフ描画の基本とカスタマイズ。
- [`leaflet_folium_jupyterlite_tutorial.ipynb`](./leaflet_folium_jupyterlite_tutorial.ipynb) — Folium/Leaflet による地図表示（名古屋市立大学経済学部を中心としたサンプル）。
- [`leaflet_folium_jupyterlite_tutorial_tokai.ipynb`](./leaflet_folium_jupyterlite_tutorial_tokai.ipynb) — Folium/Leaflet の発展編（東海4県の GeoJSON 表示）。
- [`statsmodels_jupyterlite_tutorial_v2.ipynb`](./statsmodels_jupyterlite_tutorial_v2.ipynb) — 回帰分析と統計モデリングの実践。
- [`scipy_stats_beginner_tutorial.ipynb`](./scipy_stats_beginner_tutorial.ipynb) — scipy.stats 初級：記述統計、確率分布、正規分布、乱数生成。
- [`scipy_stats_intermediate_tutorial.ipynb`](./scipy_stats_intermediate_tutorial.ipynb) — scipy.stats 中級：仮説検定、相関分析、ノンパラメトリック検定、分散分析。
- [`numpy_beginner_tutorial.ipynb`](./numpy_beginner_tutorial.ipynb) — NumPy 初級：配列の作成、インデックス、演算、統計関数。
- [`numpy_intermediate_tutorial.ipynb`](./numpy_intermediate_tutorial.ipynb) — NumPy 中級：線形代数、ブロードキャスト、構造化配列、パフォーマンス最適化。
- [`seaborn_beginner_tutorial.ipynb`](./seaborn_beginner_tutorial.ipynb) — seaborn 初級：分布の可視化、カテゴリカルプロット、回帰プロット。
- [`seaborn_intermediate_tutorial.ipynb`](./seaborn_intermediate_tutorial.ipynb) — seaborn 中級：FacetGrid、PairGrid、クラスターマップ、高度なカスタマイズ。
- [`sklearn_beginner_tutorial.ipynb`](./sklearn_beginner_tutorial.ipynb) — scikit-learn 初級：前処理、線形回帰、分類、モデル評価、交差検証。
- [`sklearn_intermediate_tutorial.ipynb`](./sklearn_intermediate_tutorial.ipynb) — scikit-learn 中級：アンサンブル学習、ハイパーパラメータチューニング、パイプライン、クラスタリング、次元削減。

Notebook 以外のデータや画像を追加する場合は Notebook 名と同じプリフィックスのサブディレクトリを作成し、トップレベルを整理します。

## エンドユーザ向け：チュートリアルの使い方

### 収録コンテンツ

| ファイル | 内容 |
|---------|------|
| [`jupyterlite_beginner_tutorial_with_exercises_v2.ipynb`](./jupyterlite_beginner_tutorial_with_exercises_v2.ipynb) | JupyterLite の基本操作と演習問題 |
| [`pandas_beginner_tutorial.ipynb`](./pandas_beginner_tutorial.ipynb) | pandas 初級：Series/DataFrame の基本、選択、フィルタリング |
| [`pandas_intermediate_tutorial.ipynb`](./pandas_intermediate_tutorial.ipynb) | pandas 中級：groupby、欠損値処理、結合、時系列 |
| [`pandas_jupyterlite_tutorial.ipynb`](./pandas_jupyterlite_tutorial.ipynb) | DataFrame の整形と集約テクニック |
| [`matplotlib_beginner_tutorial.ipynb`](./matplotlib_beginner_tutorial.ipynb) | matplotlib 初級：折れ線、散布図、棒グラフ、ヒストグラム |
| [`matplotlib_intermediate_tutorial.ipynb`](./matplotlib_intermediate_tutorial.ipynb) | matplotlib 中級：サブプロット、軸設定、seaborn連携 |
| [`matplotlib_jupyterlite_tutorial.ipynb`](./matplotlib_jupyterlite_tutorial.ipynb) | グラフ描画の基本とカスタマイズ |
| [`leaflet_folium_jupyterlite_tutorial.ipynb`](./leaflet_folium_jupyterlite_tutorial.ipynb) | Folium/Leaflet による地図表示 |
| [`leaflet_folium_jupyterlite_tutorial_tokai.ipynb`](./leaflet_folium_jupyterlite_tutorial_tokai.ipynb) | Folium/Leaflet 発展編（東海4県 GeoJSON） |
| [`statsmodels_jupyterlite_tutorial_v2.ipynb`](./statsmodels_jupyterlite_tutorial_v2.ipynb) | 回帰分析と統計モデリング |
| [`scipy_stats_beginner_tutorial.ipynb`](./scipy_stats_beginner_tutorial.ipynb) | scipy.stats 初級：記述統計、確率分布、正規分布 |
| [`scipy_stats_intermediate_tutorial.ipynb`](./scipy_stats_intermediate_tutorial.ipynb) | scipy.stats 中級：仮説検定、相関分析、分散分析 |
| [`numpy_beginner_tutorial.ipynb`](./numpy_beginner_tutorial.ipynb) | NumPy 初級：配列の作成、インデックス、統計関数 |
| [`numpy_intermediate_tutorial.ipynb`](./numpy_intermediate_tutorial.ipynb) | NumPy 中級：線形代数、ブロードキャスト、パフォーマンス |
| [`seaborn_beginner_tutorial.ipynb`](./seaborn_beginner_tutorial.ipynb) | seaborn 初級：分布・カテゴリカル・回帰の可視化 |
| [`seaborn_intermediate_tutorial.ipynb`](./seaborn_intermediate_tutorial.ipynb) | seaborn 中級：FacetGrid、クラスターマップ |
| [`sklearn_beginner_tutorial.ipynb`](./sklearn_beginner_tutorial.ipynb) | scikit-learn 初級：前処理、回帰、分類、評価 |
| [`sklearn_intermediate_tutorial.ipynb`](./sklearn_intermediate_tutorial.ipynb) | scikit-learn 中級：アンサンブル、チューニング、クラスタリング |

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
- 2025-12-02: NumPy、seaborn、scikit-learn の初級・中級チュートリアルを追加。
- 2025-12-02: scipy.stats 初級・中級チュートリアルを追加（`scipy_stats_beginner_tutorial.ipynb`, `scipy_stats_intermediate_tutorial.ipynb`）。
- 2025-12-02: matplotlib 初級・中級チュートリアルを追加（`matplotlib_beginner_tutorial.ipynb`, `matplotlib_intermediate_tutorial.ipynb`）。
- 2025-12-02: pandas 初級・中級チュートリアルを追加（`pandas_beginner_tutorial.ipynb`, `pandas_intermediate_tutorial.ipynb`）。
- 2025-12-02: エンドユーザ向けチュートリアル利用ガイドを追加。収録コンテンツ一覧の表形式化、利用方法・学習の進め方を整備。
- 2025-11-24: R 統計演習用 Notebook (`jupyterlite_xeus_r_stats_practice.ipynb`) を追加。
- 2025-11-21: 初版公開。各種 JupyterLite チュートリアルと `AGENTS.md` を追加。
  - 重複ファイル `leaflet_folium_jupyterlite_tutorial (1).ipynb` を削除。
  - `leaflet_folium_jupyterlite_tutorial.ipynb` のサンプル座標を浜松市から名古屋市立大学経済学部（滝子キャンパス）に変更。
  - 各ファイルの緯度経度の記述ミスを修正。
  - `leaflet_folium_jupyterlite_tutorial_tokai.ipynb` を追加（東海4県の GeoJSON 表示の発展編）。
