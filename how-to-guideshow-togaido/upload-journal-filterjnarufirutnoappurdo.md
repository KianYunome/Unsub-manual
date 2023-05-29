# Upload journal filter(ジャーナルフィルターのアップロード)

Any Unsub dashboard supports journals from any publisher. However, Unsub started off with each dashboard being concerned with one publisher. Thus, you may be used to, for example, uploading COUNTER reports for Elsevier and be expecting to see only Elsevier journals in your dashboard.(Unsubダッシュボードは、どの出版社のジャーナルもサポートします。しかし、Unsubは当初、各ダッシュボードが1つの出版社を対象としていました。そのため、例えばElsevierのCOUNTERレポートをアップロードしている場合、ダッシュボードにはElsevierのジャーナルしか表示されないと思っているかもしれません。)

As we now support all publishers - including a mix of publishers - we no longer filter titles in a dashboard by publisher. All titles are included from COUNTER report you upload as long as they do not fall under one or more of these three reasons.(現在では、すべての出版社（複数の出版社を含む）をサポートしているため、ダッシュボードで出版社ごとにタイトルをフィルタリングすることはありません。アップロードしたCOUNTERレポートには、\[these three reasons(3つの理由)]\(../troubleshooting/why-dont-i-see a certain-title-in-my-dashboard.md) に当てはまらない限り、すべてのタイトルが含まれます。)

To address the lack of filtering by publisher, we now support user supplied title filtering. Filtering titles is **optional**.(出版社によるフィルタリングの不足を解消するため、ユーザーによるタイトルのフィルタリングをサポートするようになりました。タイトルのフィルタリングは **optional** です。)

### Filtering titles(タイトルのフィルタリング)

First, navigate to the package you're interested in, click the Setup tab, and scroll to the Filter section:(まず、興味のあるパッケージに移動し、Setup(設定)タブをクリックし、Filter(フィルター)セクションまでスクロールします。)

As you can see, there is a warning that you are missing data.(ご覧のように、データが不足している旨の警告が表示されます。)

If you upload a KBART file, make sure to edit the file to only the ISSNs you want to whitelist.(KBARTファイルをアップロードする場合は、ホワイトリストに登録したいISSNのみにファイルを編集するようにしましょう。)

Let's fix that by uploading a custom file. The file is pretty simple, just a spreadsheet with one column: **ISSN**.(カスタムファイルをアップロードして修正しましょう。ファイルは非常にシンプルで、1つのカラムを持つ単なるスプレッドシートです。**ISSN**です。)

Here's an example:(以下にサンプルを提示します。)

To upload your file, click the Paperclip, then find your file and select it, then click the Upload arrow. You'll wait a minute or two while Unsub starts to upload and process the file. Then when it's done, you'll see something like this:(ファイルをアップロードするには、Paperclipをクリックし、ファイルを探して選択し、アップロードの矢印をクリックします。Unsubがファイルをアップロードして処理する間、1～2分ほど待ちます。アップロードが完了すると、このような画面が表示されます。)

We can see there were 250 rows of useful data. You can click on the download arrow to the far right to view the journals used to filter the titles in your your dashboards.(250行の有用なデータがあることがわかります。右端のダウンロード矢印をクリックすると、ダッシュボードでタイトルをフィルタリングするために使用したジャーナルを表示できます。)

If you'd like to replace this data later you can click the Trash can to the right of the row and then upload a new file — your scenario forecasts will automatically recalculate to use the new data.(もし、このデータを後で交換したい場合は、行の右側にあるゴミ箱をクリックし、新しいファイルをアップロードしてください。)

Upon returning to any scenario within the package you should now see a blue message "Journal Whitelist (some number)" in the upper right hand corner. For example:(パッケージ内のシナリオに戻ると、右上に "Journal Whitelist (some number) "という青いメッセージが表示されるはずです。例えば、以下のようになります。)

You can click on the blue "Journal Whitelist" text to get to this documentation page.("Journal Whitelist"の青いテキストをクリックすると、このドキュメント・ページにアクセスできます。)

Importantly, the titles that you see in your dashboard may not match exactly to the titles uploaded in the Journal Filter setup step. These are some of the situations you could encounter after filtering:(重要なのは、ダッシュボードに表示されるタイトルが、Journal Filterの設定ステップでアップロードしたタイトルと完全に一致しない場合があります。このような状況は、フィルタリング後に発生する可能性があります。)

* The number of titles in your scenario is unchanged. This could be because the titles you filtered to matched exactly the titles already in your dashboard.(The number of titles in your scenario is unchanged(シナリオのタイトル数は変更されません。)これは、フィルタリングしたタイトルが、ダッシュボードに既にあるタイトルと正確に一致したためと思われます。)
* The number of titles in your scenario has gone down but you still have some titles. This should be the most common case.(The number of titles in your scenario has gone down but you still have some titles.(シナリオのタイトル数は減少しているが、まだいくつかのタイトルがある。)これは、最も一般的なケースです。)
* There are no titles in your dashboard. This could happen if you filter by ISSNs that are valid, but do match any titles in your dashboard.(There are no titles in your dashboard.(ダッシュボードにタイトルがない。)これは、有効なISSNでフィルタリングした場合に発生する可能性がありますが、ダッシュボードの任意のタイトルと一致します。)

If you have a different situation, or any questions about any of this please get in touch at [support@unsub.org](mailto:support@unsub.org)(もし、上記と異なる状況やご質問がありましたら、[support@unsub.org](mailto:support@unsub.org)までご連絡ください。)
