# Upload title prices(タイトル毎の価格のアップロード)

A key data source for Unsub is the title-by-title price for each journal — the actual real-world cost you'll pay, if you choose to subscribe to that journal individually outside any Big Deal. For any given journal, there are two sources for the title-by-title price:(Unsubの主要なデータソースは、各ジャーナルのタイトル別価格です。これは、ビッグディール以外でそのジャーナルを個別に購読する場合、実際に支払うコストです。各ジャーナルのタイトル別価格には、2つの情報源があります。)

1. **Custom uploaded price:** You can upload a simple spreadsheet with custom prices for each journal. Any custom prices you upload will be interpreted in the currency you have chosen for your package.(**Custom uploaded price:** 各ジャーナルのカスタム価格を簡単なスプレッドシートでアップロードすることができます。アップロードしたカスタム価格は、お客様がパッケージに選択した通貨で計算されます。)
2. **No price:** If you didn't upload a list price for a journal, then the price is unknown. In that case, this journal will be _omitted from forecasting,_ because we don't know how they will affect the financial side of the model.(**No price:(価格なし)** ジャーナルの定価をアップロードしなかった場合、価格は不明となります。その場合、このジャーナルは予測から除外されます。)

{% hint style="info" %}
Public list price: We used to provide public list prices. We no longer provide them. See the Getting Title Prices page for help.(公示価格です。以前は定価を公開していました。現在では提供していません。Getting Title Prices(タイトル価格の入手) ページを参照してください。)
{% endhint %}

You can see the source of price data for each journal by going to your institution page, clicking the package you are interested in, opening the Setup tab, and then clicking the "Pricelist" section.(各ジャーナルの価格データのソースは、自機関のページで、興味のあるパッケージをクリックして、Setupタブを開き、"Pricelist"セクションをクリックすることで確認することができます。)

If you don't have any title prices uploaded, you will see one of two screens:(タイトル価格がアップロードされていない場合、次の2つの画面のうちどちらかが表示されます)

* COUNTER reports **have not been uploaded**. The message on the pricelist page states simply that pricelist data is required.(\* COUNTERレポートが**have not been uploaded(アップロードされていません)**。pricelistのページのメッセージは、単にpricelistのデータが必要であることを述べています。)
* COUNTER reports **have been uploaded**. The message states that the pricelist data is required, and tells you how many titles are missing price information.(COUNTERレポートが**have been uploaded(アップロードされました)**。メッセージには、pricelistデータが必要であることと、価格情報が不足しているタイトルの数が表示されます。)

If you click on "View Missing Titles", you will download a spreadsheet with the ISSNs, Titles, and an approximate sum of your COUNTER data for that title (column named "counter\_total") so that you know how important it is to you to make sure you get the price reflected in your Unsub dashboard. The "counter\_total" column includes only data from your COUNTER reports; it does not include citations or authorships data that you see in the Unsub dashboard. The file looks like:("View Missing Titles" をクリックすると、ISSN、タイトル、そのタイトルの COUNTER データの概算合計 (カラム名 "counter\_total") を含むスプレッドシートがダウンロードされるので、Unsub ダッシュボードに反映される価格を確認することがいかに重要であるかがわかります。"counter\_total "カラムはCOUNTERレポートのデータのみを含み、Unsubダッシュボードに表示される引用や著者のデータは含まれません。ファイルは以下のようなものです。)

Once you have your price data available, the format needed for Unsub is really simple. It's just two columns: **ISSN** and **Price**. You include a row for every journal where you have a custom price to set. The prices are interpreted in the Currency you set in your Package Setup (currency symbols are ignored). The file needs to be in .csv, .xlsx, or .xls format with just one sheet. Files can not contain formulas or other non value contents. We don't currently handle files that have non-value contents like formulas. Here's an example:(価格データを入手したら、Unsubに必要なフォーマットはとてもシンプルです。2つのカラムだけです。**ISSN** と **Price** です。カスタム価格を設定するジャーナルごとに行を追加します。価格は、パッケージ設定で設定した通貨で計算されます（通貨記号は無視されます）。ファイルは.csv、.xlsx、または.xls形式で、1つのシートだけである必要があります。ファイルには、数式やその他の値以外の内容を含めることはできません。現在、数式などの値でない内容を含むファイルは扱えません。以下はその例です。)

{% hint style="danger" %}
Do not use a thousands comma or period separator in the Price column(価格欄にはカンマやピリオドなどの区切り文字を使用しないでください。)
{% endhint %}

To upload, just click the Upload button, then click the Paperclip, find your file and select it, then click the Upload arrow. You'll wait a minute or two while Unsub starts to upload and process the file. Then when it's done, you'll see something like this:(アップロードするには、アップロードボタンをクリックし、Paperclipをクリックし、ファイルを見つけて選択し、アップロードの矢印をクリックするだけです。Unsubがファイルをアップロードして処理する間、1、2分ほど待ちます。アップロードが完了すると、このような画面が表示されます。)

If you want to see the prices you have uploaded you can click the download button on the far right of the file row. If you'd like to replace your Custom journal pricelist, click the garbage can to the right of the file row and then upload your new file.(アップロードした価格を確認したい場合は、ファイル列の右端にあるDownloadボタンをクリックします。カスタムジャーナルの価格表を差し替えたい場合は、ファイル行の右側にあるゴミ箱をクリックし、新しいファイルをアップロードしてください。)

Note that the red alert has given way to an orange alert - indicating that required data has been uploaded but that there are still missing prices.(赤のアラートがオレンジのアラートに変わったのは、必要なデータはアップロードされているが、不明な価格があることを示しています。)

If you do happen to get all title prices you will see something like the screen below with a green alert and check mark:(もし、すべてのタイトル価格を取得することができた場合、以下の画面のように緑色のアラートとチェックマークが表示されます。)

{% hint style="info" %}
Unsub only supports pricing at the single-journal level. For more on how to address mini-bundle pricing see this article.(Unsubは単一ジャーナルレベルの価格設定にのみ対応しています。ミニバンドル価格への対応については、this article(この記事)をご覧ください。)
{% endhint %}
