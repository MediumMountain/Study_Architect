# COCOMOによるプロジェクト工数の見積もり

# COCOMO法（パラメトリック法）
- ソフトウェア開発の工数・期間の見積もり手法。
    - 予想されるプログラム行数にエンジニアの能力や要求の信頼性などの補正係数を掛け合わせて開発工数や期間，要員や生産性を見積もる手法
- 1981年にバリー・ベーム（Barry Boehm）博士が提唱した。

- 具体的には開発するソフトウェアの予想されるコード行数に、エンジニアの能力や要求の信頼性といった補正係数を掛け合わせて（名目工数×努力係数）、開発に必要な工数、期間、要員、生産性を算出する。
- 実装言語の違いに左右されず、客観的な数値を算出できるといわれている。
- また基本の数式モデルについても、実際のプロジェクトにおける適用結果をフィードバックし、精緻化を重ねている。

```
COCOMOを適用するには自社における生産性のデータ収集が不可欠
```


## 3つのモデル
- COCOMOは次の3つのモデルが存在する。

| モデル | 説明 | 
|:--:|:--:|
|基本COCOMO |	早期の段階で適用できるモデル、単純な回帰式 |
|中間COCOMO |要求定義終了時に適用するモデル、工数変動要因を考慮、重回帰式 |
|詳細COCOMO | 設計終了後に適用するモデル、工程ごとの見積り算出が可能 |

## 基本COCOMO (Basic COCOMO)
- 基本モデルでは、次に示す2つの要因から工数(人月)を見積もる。
- 規模から単純に工数を導出：
```
Effort=α×Sizeb
```

1. 見積もり対象プロジェクトのモード
1. 開発するソフトウェアの予想されるソースコード行数(LOC: Lines of code)

- 見積もり要因が少ないことから、基本モデルはプロジェクト早期の段階で適用することができる。
- ただし、中間モデルや詳細モデルと比べて見積もり精度は劣る。
- ソースコード行数は、過去の類似プロジェクトでの実績やファンクションポイント法などから見積もる必要がある。
- COCOMOでは、見積もり対象プロジェクトを次の3つのモードに分類している。


### 基本COCOMOモデルにおける見積り式
|モード	|工数(人月)|開発期間(月)|
|:--:|:--:|:--:|
|組織	|2.4･kloc1.05|2.5･effort0.38|
|半組込	|3.0･kloc1.12|2.5･effort0.35|
|組込	|3.6･kloc1.20|2.5･effort0.32|


## 中間COCOMO (Intermediate COCOMO)
システムの開発特性を考慮：
```
Effort=α×Sizeb×Πβ
```

### 中間COCOMOにおける工数(人月)見積り式
|モード|	工数見積り式|
|:--:|:--:|
|半組込|	2.4・kloc1.05・ΠA|
|組織	|3.0・kloc1.12・ΠA|
|組込|	3.6・kloc1.20・ΠA|

※ΠA = A1 * A2 * A3 * A4 * A5 * A6 * A7 * A8 * A9 * A10 * A11 * A12 * A13 * A14 * A15




### 詳細COCOMO

- 中間COCOMOからさらにモジュールレベルでの見積りが可能



### モード
- 組織モード：自社開発のような熟練度の高い開発形態を指し、少人数の開発チームで在庫管理システムや科学技術計算用パッケージなどの業務アプリケーションを開発する場合

- 組込モード：開発チームが大規模であり、種々の厳しい制約条件のもとでハードウェア、ソフトウェア、運用手順などの複雑さがからみ合っている場合
- 半組込みモード：組織モードと組込みモードの中間




## REFERENCE
https://segakuin.com/management/cocomo.html
https://www.ipa.go.jp/archive/digital/iot-en-ci/ent01-c.html
https://www.itmedia.co.jp/im/articles/0308/14/news004.html