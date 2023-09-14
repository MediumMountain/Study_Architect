# プレシデンスダイアグラム法(PDM法)
- 個々の作業を四角で囲み、作業同士を矢印で結ぶことで作業順序や依存関係を表現する図法です。

- 作業同士の関係を表すという意味ではアローダイアグラムと同じですが、アローダイアグラムでは作業を矢印で結合点を丸のノードで示すので、記述方法が根本的に異なります。
- またアローダイアグラムでは、ある作業の終了が別の作業の開始条件となる「終了-開始」(FS：Finish to Start)の依存関係しか表現できませんが、プレシデンスダイアグラムでは「開始」と「終了」を組み合わせた4つの依存関係を記述することができます。

## FF関係（Finish-to-Finish，終了-終了）
- 「受付が終了したら試験会場への入場を終了する」というように、あるアクティビティの終了が、他方のアクティビティの終了条件になっている関係

## FS関係（Finish-to-Start，終了-開始）
- 「受付が終了してから試験を開始する」というように、あるアクティビティの終了が、他方のアクティビティの開始条件になっている関係

## SF関係（Start-to-Finish，開始-終了）
- 「試験が開始されたら受付を終了する」というように、あるアクティビティの開始が、他方のアクティビティの終了条件になっている関係

## SS関係（Start-to-Start，開始-開始）
- 「受付が開始されたら試験会場への入場を開始する」というように、あるアクティビティの開始が、他方のアクティビティの開始条件になっている関係


## 「リード」と「ラグ」
- 先行アクティビティに対して、後続アクティビティの開始を前倒しや後ろ倒しする制約がある場合にその時間を表すものです。

### リード
- 先行アクティビティに対して、後続アクティビティの開始を前倒しできる時間
### ラグ
- 先行アクティビティに対して、後続アクティビティの開始を遅らせる時間



![PDM](https://github.com/MediumMountain/\Study_Architect/blob/main/PICTURE/Manage/PDM_1.png)
![PDM](https://github.com/MediumMountain/\Study_Architect/blob/main/PICTURE/Manage/PDM_2.png)

![PDM_arrow](https://github.com/MediumMountain/\Study_Architect/blob/main/PICTURE/Manage/PDM_arrow_1.png)
![PDM_arrow](https://github.com/MediumMountain/\Study_Architect/blob/main/PICTURE/Manage/PDM_arrow_2.png)