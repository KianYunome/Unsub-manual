# What does the "Missing Prices" warning mean?
# "Missing Prices" の警告は何を意味するのでしょうか？

Do you have a warning like this at the top of your Forecast Scenario?
Forecast Scenarioのトップにこのような警告が表示されることはありませんでしょうか？

![](../.gitbook/assets/missing-prices.png)

If so, it's because we don't know the subscription price for some of the journals in your COUNTER reports.
もしそうなら、COUNTERレポートにあるいくつかの雑誌の購読料金がわからないためこのような警告が表示されます。

We'd like to include these journals in the forecast scenario, but we can't, because without a title-level subscription price, we can't calculate its title-level cost per use.
これらのジャーナルを予測シナリオに含めたいのですが、タイトルレベルの購読料金がなければ、そのタイトルレベルのCost per use(利用毎単価)を計算できないため、予測シナリオに含めることができません。

So, **any journals with missing prices are omitted from your forecasting dashboards.** That makes the forecasting less useful to you, since we're just ignoring some journals that might be important.
つまり、**any journals with missing prices are omitted from your forecasting dashboards.(価格が見つからないジャーナルは、予測ダッシュボードから省かれます。)**それでは、重要かもしれないジャーナルを無視することになり、予測の有用性は低くなってしまいます。

That means you'll need to contact your sales representative to get a quote for these missing prices.
つまり、これらの欠落したジャーナルの価格は、販売担当者に問い合わせる必要があります。

To find out which journals are missing prices: go to the Package page (you can click its name in the top left corner of your screen), then view the Setup tab, and finally select the "Pricelist" menu option. Click "View Journals" to download a spreadsheet showing the missing journals. These are the ones you'll need to ask a quote for.
どのジャーナルの価格が足りないかを調べるには：the Package page：パッケージページ（画面左上の名前をクリックできます）に行き、セットアップタブを表示し、最後に"Pricelist(価格表)"メニューオプションを選択します。"View Journals(ジャーナルを見る)"をクリックすると、不足しているジャーナルを示すスプレッドシートがダウンロードできます。これらは、個別ジャーナルの見積もりを依頼する必要がある時に利用します。

![](../.gitbook/assets/prices-setup-with-counter-withcustom.png)

Once you've got price quotes for the missing titles, you can then upload a custom Journal Pricelist file and resolve the warning. See [this article](../how-to-guides/upload-title-prices.md) for details on how to format and upload your Pricelist file.
不足するタイトルの価格見積もりができたら、Journal Pricelist fileをカスタムでアップロードして警告を解決することができます。Pricelistファイルのフォーマットとアップロード方法の詳細は、[this article(この記事)](../how-to-guides/upload-title-prices.md)を参照してください。
