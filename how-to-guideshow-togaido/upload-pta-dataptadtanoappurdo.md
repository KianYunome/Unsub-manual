# Upload PTA data(PTAデータのアップロード)

A key data source for Unsub is the Post-Termination Access dates of each journal — the range of content you'll still have access to, even after a cancellation. If you cancel a Big Deal, PTA to back content will become an important source of fulfillment, especially over the first few years.(Unsubの重要なデータソースは、各ジャーナルのPost-Termination Access Date（解約後もアクセス可能なコンテンツの範囲）です。ビッグディールをキャンセルした場合、特に最初の数年間は、バックコンテンツへのPTAが重要なコンテンツへのFulfillment（利用実現可能性）の源になります。)

Of course, this will vary, depending on the journal. In some fields (like math or philosophy), back content stays relevant for a long time, and so PTA is quite significant. In other (like biomed), readers are disproportionately reading brand-new articles, and so PTA doesn't impact post-cancellation fulfillment that much. The Unsub model accounts for all this, using a training set composed of millions of data points from thousands of libraries, and customized it to your institution using your COUNTER data.(もちろん、これはジャーナルによって異なります。数学や哲学のように、バックコンテンツが長期間にわたって関連性を持ち続ける分野では、PTAは非常に重要です。一方、（生物医学のように）読者が読むのは圧倒的に新しい論文の場合は、PTAは解約後のFulfillment(利用実現可能性)にそれほど影響を与えません。Unsubモデルは、何千もの図書館から集められた何百万ものデータからなるトレーニングデータセットを使用して、これらすべてを考慮し、COUNTERデータを使用して自機関用にカスタマイズされています。)

**By default, the model assumes that you have no PTA rights to any of the journals in your COUNTER data**. However, this is probably not the case, and so **likely underestimates your post-cancellation access**. You can upload a list of your actual PTA date ranges by journal, and Unsub will recalculate your forecasts using that data.(**By default, the model assumes that you have no PTA rights to any of the journals in your COUNTER data(デフォルトでは、このモデルはあなたのCOUNTERデータ内のどのジャーナルに対してもPTAの権利を持っていないと仮定しています)**。しかし、これはおそらく事実ではないため、**likely underestimates your post-cancellation access(ビッグディール解約後のアクセスを過小評価する可能性があります)**。ジャーナルごとの実際のPTAの日付範囲のリストをアップロードしていただければ、Unsubはそのデータを使って予測を再計算します。)

Here's how.(その方法を説明します。)

First, navigate to the package you're interested in, click the Setup tab, and scroll to the PTA section:(まず、興味のあるパッケージに移動し、「Setup」タブをクリックし、「PTA」セクションまでスクロールします。)

As you can see, there is a warning that you are missing PTA data.(ご覧のように、PTAデータが不足しているという警告が表示されています。)

Let's fix that by uploading a custom file. The file is pretty simple, just a spreadsheet with three columns: **ISSN**, **Start Data**, and **End Date**. A few other tips:(カスタムファイルをアップロードすることで、それを修正しましょう。このファイルは非常にシンプルで、3つの列を持つスプレッドシートだけです。**ISSN**, **Start Data**, and **End Date**. その他のヒントをいくつか紹介します。)

* For the dates, we prefer an [ISO 8601](https://en.wikipedia.org/wiki/ISO\_8601) format like this: **YYYY-MM-DD**. However, we make our best guess at dates in other formats as well, and they generally work.(日付は、以下のような [ISO 8601](https://en.wikipedia.org/wiki/ISO\_8601) 形式が望ましいです。**yyyy-mm-dd**. しかし、他の形式の日付も可能な限り推測しており、一般的に有効です。)
* If a journal's PTA is ongoing, leave the End Date blank.(ジャーナルのPTAが進行中の場合、End Dateは空白のままにしてください。)

Here's an example:(以下はその例となります)

To upload your file, click the Paperclip, then find your file and select it, then click the Upload arrow. You'll wait a minute or two while Unsub starts to upload and process the file. Then when it's done, you'll see something like this:(ファイルをアップロードするには、Paperclipをクリックし、ファイルを見つけて選択し、Uploadの矢印をクリックします。Unsubがファイルをアップロードして処理する間、1〜2分ほど待ちます。アップロードが完了すると、このような画面が表示されます。)

Looking at the "Your PTA file" section, we can see there are now 373 journals where the model will using our custom date ranges. You can click on the download arrow to the far right to view the journals and the ranges being used.(Your PTA fileセクションを見ると、現在373のジャーナルがあり、カスタム日付範囲を使用するモデルになっていることがわかります。右端のダウンロード矢印をクリックすると、使用されているジャーナルと範囲を表示できます。)

If you'd like to replace this data later you can click the Trash can to the right of the row and then upload a new file — your scenario forecasts will automatically recalculate to use the new data.(もし、後でこのデータを置き換えたい場合は、行の右側にあるゴミ箱をクリックし、新しいファイルをアップロードすることができます - シナリオ予測は自動的に新しいデータを使用して再計算されます。)

### A few things to be aware of related to PTA in Unsub(UnsubのPTAに関連するいくつかの注意点)

* Unsub forecasts only use PTA back to 2012. If you have PTA start dates before 2012, we will not use them. There's no need to edit your PTA file - just be aware that start dates prior to 2012 will be converted to 2012.(Unsubの予測では、2012年までのPTAしか使用しません。2012年以前のPTA開始日がある場合は、使用されません。PTAファイルを編集する必要はありません。ただ、2012年より前の開始日は2012年に変換されることに注意してください。)
* For PTA end dates that are ongoing (blank) or greater than the current year (e.g. 2023 if the year is 2022), we will set the end date to be the current year minus one. For example, if your PTA end date for a title is blank, 2022, or any year greater than 2022, the end date you'll see for that title will be 2021.(PTA の終了日が現在進行中（空白）または現在の年よりも大きい場合（例えば、年が 2022 年の場合は 2023 年）、終了日は現在の年から 1 を引いた値に設定されます。例えば、あるタイトルのPTA終了日が空白、2022年、または2022年より大きい年の場合、そのタイトルの終了日は2021と表示されるでしょう。)

\\
