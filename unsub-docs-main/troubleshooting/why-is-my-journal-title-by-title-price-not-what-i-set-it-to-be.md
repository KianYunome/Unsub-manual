---
description: >-
  Handling difference between uploaded title-by-title price, and the price as
  displayed in the forecast scenarios
  アップロードされたタイトルごとの価格と、予測シナリオに表示される価格との差分を処理します。予測シナリオに表示される価格の違いを処理する
---

# Why is my journal title-by-title price not what I set it to be?
# なぜジャーナルのタイトルごとの価格は私が設定したものではないのでしょうか？

**Problem**: in the Publisher Setup tab, you've uploaded a title-by-title Journal Pricelist. Let's say you've uploaded a price of $1000 for The Journal of Example Studies.
**問題**： Publisher Setup（出版社設定）タブで、タイトルごとのJournal Pricelist（ジャーナル価格リスト）をアップロードしました。例えば、The Journal of Example Studiesの価格を$1000とアップロードしたとします。

Then you go to the forecast scenario, and look at the same journal--but the price is higher.
次に、予測シナリオで同じジャーナルを見ますが、価格はもっと高くなっています。

**Solution**: The price you uploaded is the _current_ annual price of the journal.
**解決方法**。アップロードした価格は、その雑誌の現在の年間価格です。

But on the scenario page, we're looking at your _forecasted_ annual price of this journal, averaged over the next five years. Everything in the Scenario view is about the future state of the world, over the next five years....specifically it's looking at the one-year average over the next five years.
しかし、シナリオのページでは、この雑誌の今後5年間の平均的な年間価格（予測）を見ているのです。シナリオ・ビューのすべては、今後5年間の、世界の未来の状態についてです...具体的には、今後5年間の1年平均を見ているのです。

The number in the scenario view is higher because, over the next five years, you will probably pay a higher price for this journal than you do now. When we forecast future journal prices, we include a term to model year-on-year increase in price. By default this is 8% (based on historical trends), but you can set it to any number you like, including 0%, by clicking Parameters➞Costs➞Title-by-title subscription cost growth.
シナリオ・ビューの数値が高いのは、今後5年間で、このジャーナルの価格が今よりも高くなる可能性が高いからです。将来のジャーナル価格を予測する際、前年比の価格上昇をモデル化する期間を入れています。デフォルトでは8%（過去のトレンドに基づく）ですが、パラメータ➞コスト➞タイトルごとの購読コスト上昇をクリックすれば、0%を含む任意の数値に設定できます。

![](../.gitbook/assets/title-price-not-what-set-to-be.png)
