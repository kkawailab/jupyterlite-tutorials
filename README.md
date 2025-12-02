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

### 練習問題集
- [`python_beginner_exercises_30.ipynb`](./python_beginner_exercises_30.ipynb) — 初級練習問題30題：Python基礎、NumPy、Pandas、Matplotlib、Seaborn、SciPy、Scikit-learn。
- [`python_intermediate_exercises_30.ipynb`](./python_intermediate_exercises_30.ipynb) — 中級練習問題30題：線形代数、groupby、サブプロット、仮説検定、アンサンブル学習など。

Notebook 以外のデータや画像を追加する場合は Notebook 名と同じプリフィックスのサブディレクトリを作成し、トップレベルを整理します。

## エンドユーザ向け：チュートリアルの使い方

### JupyterLite とは？

JupyterLite は、**ブラウザだけで動く Jupyter 環境**です。通常の Jupyter Notebook は Python のインストールやサーバーの起動が必要ですが、JupyterLite ではそれらが一切不要です。

**JupyterLite のメリット**：
- インストール不要：ブラウザで URL を開くだけで使える
- どこでも同じ環境：PC、タブレット、スマートフォンから利用可能
- 安全：コードはすべてブラウザ内で実行され、サーバーにデータが送られない
- 初心者に優しい：環境構築でつまずくことがない

### Notebook の基本操作

Jupyter Notebook は「セル」と呼ばれる単位でコードや説明文を管理します。

#### セルの種類
| セルの種類 | 用途 | 見分け方 |
|-----------|------|---------|
| コードセル | Python コードを書いて実行する | 左側に `[ ]:` または `[1]:` のような番号がある |
| マークダウンセル | 説明文や見出しを書く | 実行すると整形されたテキストになる |

#### 基本的なキーボードショートカット

| 操作 | ショートカット | 説明 |
|------|---------------|------|
| セルを実行 | `Shift + Enter` | 現在のセルを実行し、次のセルに移動 |
| セルを実行（移動なし） | `Ctrl + Enter` | 現在のセルを実行し、そのセルにとどまる |
| 上にセルを追加 | `A` | コマンドモードで押すと、上に新しいセルを追加 |
| 下にセルを追加 | `B` | コマンドモードで押すと、下に新しいセルを追加 |
| セルを削除 | `D` を2回 | コマンドモードで `D` を2回押すとセルを削除 |
| コードセルに変更 | `Y` | コマンドモードで押すとコードセルに変更 |
| マークダウンセルに変更 | `M` | コマンドモードで押すとマークダウンセルに変更 |
| 編集モード → コマンドモード | `Esc` | セルの編集を終了 |
| コマンドモード → 編集モード | `Enter` | セルの編集を開始 |

> **💡 ヒント**：セルの左側をクリックすると青色（コマンドモード）、セル内をクリックすると緑色（編集モード）になります。

#### セルの実行順序について

- セルは**上から順番に実行する**のが基本です
- 途中のセルをスキップすると、変数が定義されずエラーになることがあります
- エラーが出たら、まず上のセルから順番に実行し直してみてください

### 推奨学習パス

プログラミング経験に応じて、以下の順序で学習することをお勧めします。

#### 🔰 プログラミング初心者の方

```
1. jupyterlite_beginner_tutorial_with_exercises_v2.ipynb（JupyterLite の操作に慣れる）
    ↓
2. numpy_beginner_tutorial.ipynb（配列計算の基礎）
    ↓
3. pandas_beginner_tutorial.ipynb（データ操作の基礎）
    ↓
4. matplotlib_beginner_tutorial.ipynb（グラフ作成の基礎）
    ↓
5. python_beginner_exercises_30.ipynb（練習問題で復習）
```

#### 📊 データ分析を学びたい方

```
1. pandas_beginner_tutorial.ipynb → pandas_intermediate_tutorial.ipynb
    ↓
2. scipy_stats_beginner_tutorial.ipynb（統計の基礎）
    ↓
3. seaborn_beginner_tutorial.ipynb（統計的可視化）
    ↓
4. statsmodels_jupyterlite_tutorial_v2.ipynb（回帰分析）
```

#### 🤖 機械学習を学びたい方

```
1. numpy_beginner_tutorial.ipynb → numpy_intermediate_tutorial.ipynb
    ↓
2. pandas_beginner_tutorial.ipynb → pandas_intermediate_tutorial.ipynb
    ↓
3. sklearn_beginner_tutorial.ipynb → sklearn_intermediate_tutorial.ipynb
    ↓
4. python_intermediate_exercises_30.ipynb（応用問題で力試し）
```

#### 🗺️ 地理データの可視化を学びたい方

```
1. matplotlib_beginner_tutorial.ipynb（グラフの基礎）
    ↓
2. leaflet_folium_jupyterlite_tutorial.ipynb（地図表示の基礎）
    ↓
3. leaflet_folium_jupyterlite_tutorial_tokai.ipynb（GeoJSON の活用）
```

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

#### 練習問題集

| ファイル | 内容 |
|---------|------|
| [`python_beginner_exercises_30.ipynb`](./python_beginner_exercises_30.ipynb) | 初級練習問題30題（Python基礎〜Scikit-learn） |
| [`python_intermediate_exercises_30.ipynb`](./python_intermediate_exercises_30.ipynb) | 中級練習問題30題（線形代数、仮説検定、機械学習など） |

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

### よくある質問（FAQ）

<details>
<summary><strong>Q: セルを実行したのに何も表示されません</strong></summary>

**A**: 以下を確認してください：
- セルの左側に `[*]:` と表示されている場合は、まだ実行中です。少し待ってください
- 変数への代入だけのセル（例：`x = 10`）は、何も出力されないのが正常です
- 結果を表示したい場合は `print(x)` や、セルの最後に変数名だけを書いてください
</details>

<details>
<summary><strong>Q: 「NameError: name 'xxx' is not defined」というエラーが出ます</strong></summary>

**A**: その変数がまだ定義されていません。考えられる原因：
1. 変数を定義しているセルをまだ実行していない → 上のセルから順番に実行してください
2. ページをリロードした → すべてのセルを最初から実行し直してください
3. カーネルを再起動した → メニューから「Run All」を選んでください
</details>

<details>
<summary><strong>Q: グラフが表示されません</strong></summary>

**A**: JupyterLite では、グラフを表示するために以下が必要です：
```python
import matplotlib.pyplot as plt
%matplotlib inline  # この行が必要な場合があります

# グラフを描画
plt.plot([1, 2, 3], [1, 4, 9])
plt.show()  # 明示的に表示
```
</details>

<details>
<summary><strong>Q: 作業内容は保存されますか？</strong></summary>

**A**: JupyterLite の保存動作はブラウザのローカルストレージに依存します：
- `Ctrl + S`（Mac: `Cmd + S`）で手動保存できます
- ブラウザのキャッシュをクリアすると、保存内容が消える可能性があります
- 大切な作業は、メニューから「Download」を選んで `.ipynb` ファイルとしてダウンロードしておくことをお勧めします
</details>

<details>
<summary><strong>Q: 日本語が文字化けします</strong></summary>

**A**: matplotlib で日本語を表示する場合、フォント設定が必要です：
```python
import matplotlib.pyplot as plt
plt.rcParams['font.family'] = 'DejaVu Sans'  # または利用可能なフォント
```
JupyterLite 環境では日本語フォントが限られるため、チュートリアル内の指示に従ってください。
</details>

<details>
<summary><strong>Q: ライブラリをインストールできますか？</strong></summary>

**A**: JupyterLite で追加ライブラリをインストールするには：
```python
import micropip
await micropip.install('パッケージ名')
```
ただし、すべてのライブラリが JupyterLite に対応しているわけではありません。対応していないライブラリを使いたい場合は、ローカル環境での実行をお勧めします。
</details>

### トラブルシューティング

問題が解決しない場合は、以下の手順を試してください：

1. **ページをリロード**：ブラウザの更新ボタンを押す
2. **カーネルを再起動**：メニューから「Kernel」→「Restart Kernel」を選択
3. **すべてのセルを実行**：メニューから「Run」→「Run All Cells」を選択
4. **ブラウザを変更**：Chrome、Firefox、Edge など別のブラウザで試す
5. **シークレットモード**：ブラウザ拡張機能が干渉している可能性がある場合に有効

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
- 2025-12-02: 練習問題集を追加（`python_beginner_exercises_30.ipynb`, `python_intermediate_exercises_30.ipynb`）。初級30題・中級30題の計60題。
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
