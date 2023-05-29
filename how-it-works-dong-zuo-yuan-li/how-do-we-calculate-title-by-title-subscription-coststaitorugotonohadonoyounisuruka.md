# How do we calculate title-by-title subscription costs?(タイトルごとの購読料はどのように計算するか?)

A key data source for Unsub is the title-by-title price for each journal--the actual real-world cost you'll pay, should you choose to subscribe to that journal individually outside any Big Deal.(Unsubの主要なデータソースは、各ジャーナルのタイトルごとの価格です。これは、ビッグディール以外でそのジャーナルを個別に購読することを選択した場合に、施設が実際に支払うことになるコストです。)

For any given journal, there are two possible **price sources** for the title-by-title price. There are also two **price modifiers** Unsub uses to fine-tune the forecast. Putting all that together lets us predict the annual price you'll pay over the next five years, _if_ you to subscribe to a given journal.(任意のジャーナルについて、タイトルごとの価格には2つの**price sources**があります。また、Unsubでは、予測を微調整するために2つの**price modifiers**を使用します。これらを組み合わせることで、あるジャーナルを購読した場合に、今後5年間に支払うことになる年間価格を予測することができます。)

### Price sources: <a href="#price-sources" id="price-sources"></a>

**1. Custom uploaded price:** you can upload a simple spreadsheet with custom prices for each journal. Any custom prices you upload will override the default list prices. This is also how to provide prices for journals without a default price.(\*\*1. Custom uploaded price:\*\*各ジャーナルのカスタム価格を含む簡単なスプレッドシートをアップロードすることができます]\(../how-to-guides/upload-title-prices.md).アップロードされたカスタム価格は、デフォルトのリスト価格を上書きします。アップロードしたカスタム価格は、デフォルトのリスト価格より優先されます。これは、デフォルト価格のないジャーナルに価格を提供する方法でもあります。)

**2. No price:** If you haven't uploaded a custom price for a title, then the price is unknown. In that case, this journal will be _omitted from forecasting,_ because we don't know how they will affect the financial side of the model. Your scenario will show a warning.(**2. No price:** タイトルにカスタム価格をアップロードしていない場合、価格は不明です。この場合、このジャーナルは予測から除外されます。シナリオには警告が表示されます。)

### Price modifiers: <a href="#price-modifiers" id="price-modifiers"></a>

Once you've got prices, there are also two ways those prices can be modified.(価格が決まったら、その価格を変更する方法も2つあります。)

**1. Title-by-title subscription cost growth**: Unsub is designed to _forecast_ your costs and fulfillment, not just report them. To do that, we need to be able to take into account changes in subscription pricing over time. That's what this parameter does: it simply describes the percentage price increase expected every year. The default, based on industry averages, is 8%, but you can change this in your scenario's menu, under "Parameters ➞ Costs ➞ Title-by-title subscription cost growth."(**1. Title-by-title subscription cost growth**: Unsubは、コストとFulfillment(利用実現可能性)を単に報告するだけでなく、予測するように設計されています。そのためには、購読料金の時間的な変化を考慮する必要があります。このパラメータは、毎年予想される価格上昇のパーセンテージを記述するものです。業界平均に基づくデフォルトは8%ですが、シナリオメニューの "Parameters ➞ Costs ➞ Title-by-title subscription cost growth."で変更可能です。)

**2. Title-by-title content fee:** There's also a second parameter that modifies journals subscription prices, and that's the "Title-by-title content fee." This is an extra (read: hidden) fee that publishers often charge on top of their quoted subscription costs, and so it's important to account for in order to get an accurate cost estimate. By default this is set to 5.7% (a recently-reported fee for Elsevier) but again, you can edit this in the scenario's menu, under "Parameters ➞ Costs ➞ Title-by-title 'content fee.'"(\*\*2. Title-by-title content fee:\*\*また、ジャーナルの購読価格を変更する2つ目のパラメータがあり、それは "Title-by-title content fee" です。これは、出版社が購読料の見積もりに加えて請求することが多い追加料金（隠れた料金）であり、正確なコスト見積もりを得るために考慮することが重要です。デフォルトでは5.7%に設定されていますが（Elsevierの最近の報告）、シナリオメニューの "Parameters ➞ Costs ➞ Title-by-title 'content fee. "で編集することができます。)

### Putting it all together <a href="#putting-it-all-together" id="putting-it-all-together"></a>

Let's look at an example of how this all fits together; we'll call it _Journal X_. First, we'll find the current price of a title-by-title subscription by looking it up in our price table. Let's say you've uploaded a price of $1000.(ここでは、\_Journal X\_というジャーナルを例に挙げて、これらの組み合わせについて説明します。まず、タイトルごとの購読料の現在の価格を、価格表で調べます。例えば、$1000の価格をアップロードしたとしましょう。)

For year one of the five-year forecast, we'd predict you'll pay $1000 plus the 5.7% "content fee" of $57, for a total of $1,057.(5年後の1年目は、$1000に5.7%の「コンテンツ料」$57を加えて、合計$1057を支払うと予測されます。)

For year two, we also add in the 8% increase in subscription cost, giving us $1,080 for the subscription. Adding in the content fee ($61.56 now), we estimate a total of $1,141.56.(2年目は、さらに購読料の8%増を加えて、1080ドルとします。これにコンテンツ料（現在61.56ドル）を加えて、合計1,141.56ドルとします。)

For years three, four, and five, we do the same. Finally, we average all five years together to get the estimated average annual cost of title-by-title subscription.(3年目、4年目、5年目も同じように計算します。最後に、5年分をすべて平均して、タイトルごとの購読料の平均年間推定額を求めます。)
