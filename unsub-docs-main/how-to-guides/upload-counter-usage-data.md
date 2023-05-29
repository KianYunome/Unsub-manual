---
description: >-
  Enable your custom forecasting model by uploading journal-level usage
  statistics(ジャーナルレベルの利用統計データをアップロードして、カスタム予測モデルを有効にする)
---

# Upload COUNTER usage data(COUNTERレポートのアップロード)

Before you can use Unsub to analyze and forecast your subscriptions, you'll need to upload your COUNTER data. Unsub uses this to customize its forecasting model to your particular institution.(Unsubを使用してジャーナルの購読の分析と予測を行う前に、お客様のCOUNTERデータをアップロードする必要があります。Unsubはこのデータを使って、予測モデルをお客様の機関に合わせてカスタマイズします。)

To start, navigate to the Setup of your Package. The COUNTER tab will look like this:(まず、パッケージのセットアップに移動します。COUNTERタブは以下のように表示されます。)

![](../.gitbook/assets/upload-counter-data-not-loaded.png)

We recommend using COUNTER 5 data for new packages, though COUNTER 4 is still supported.(COUNTER 4も引き続きサポートされていますが、新しいパッケージにはCOUNTER 5データを使用することをお勧めします。
)

If you have previously loaded COUNTER 4 data to a package, you can easily replace it with COUNTER 5 data by deleting the existing COUNTER 4 file (click on the Trash can to its right), then pick the COUNTER 5 radio button and uploading COUNTER 5 data as described below. All your Forecast Scenario calculations will automatically update to use the new data.(COUNTER 4データをパッケージにロードした場合、既存のCOUNTER 4ファイルを削除し（右側のゴミ箱をクリック）、COUNTER 5ラジオボタンを選択し、以下の方法でCOUNTER 5データをアップロードすれば、簡単にCOUNTER 5データに交換することができます。全ての予測シナリオの計算は、新しいデータを使用するために自動的に更新されます。)

As you get your COUNTER files ready, keep this in mind:(COUNTERファイルを準備する際、以下の点に注意ください。)

* Unsub needs three COUNTER 5 files: a TR\_J2, TR\_J3, and TR\_J4 (COUNTER 4 needs a JR1)(UnsubはCOUNTER 5の3つのファイル: a TR_J2, TR_J3, TR_J4 (COUNTER 4はJR1が必要)が必要となります。)
  * In our experience for COUNTER 5 the TR\_J3 and TR_J4 files are almost always available, but the_ TR\_J2 file is sometimes not available or has no data rows in it. If you can not get a TR\_J2 file or the TR\_J2 file does not have any rows of data except the header rows you can download and use [this fake **TR\_J2** file](https://unsub-public.s3.amazonaws.com/TR\_J2.csv). It should not affect your dashboard.(COUNTER 5の経験上、TR_J3とTR_J4はほぼ入手可能ですが、TR_J2ファイルは入手できないかデータ行がない場合があります。TR_J2ファイルが入手できない場合や、TR_J2ファイルにヘッダー行以外のデータ行がない場合は、[この偽の **TR_J2** ファイル] (https://unsub-public.s3.amazonaws.com/TR_J2.csv) をダウンロードし、使用してください。ダッシュボードに影響を与えないようにする必要があります。)
* Only these file formats are supported: .**csv, .xls,** and **.xlsx**(現在以下のファイル形式のみがサポートされています。.**csv, .xls,** and **.xlsx**.)
* There can be only one sheet in the file you upload(アップロードするファイルには、収録される1つのシートのみとなります。)
* Unsub expects the COUNTER data to cover 12 months of usage. This can be calendar year 2020, calendar year 2019 (if you think your usage patterns in 2020 were particularly unusual), or any other consecutive 12 month period.(Unsubでは、COUNTERデータは12ヶ月分の使用量を想定しています。COUNTERデータは、2020年暦年、2019年暦年（2020年の使用パターンが特に異常と思われる場合）、またはその他の連続した12ヶ月間である必要があります。)
* Files can not contain formulas or other non value contents. We don't currently handle files that have non-value contents like formulas.(ファイルには、数式やその他の値以外の内容を含めることはできません。現在、数式などの非数値的な内容を含むファイルについては処理することができません。)

Once you've got your COUNTER files, you're ready to start the uploads. Click the Paperclip, select your file, and then click the Up arrow button. Unsub will begin uploading and processing the files.(COUNTERファイルを入手したら、アップロードを開始する準備が整うこととなります。Paperclipをクリックし、ファイルを選択し、上矢印ボタンをクリックします。Unsubがファイルのアップロードと処理を開始します。)

The upload and processing will take several minutes... some of these files are big! Once it is done, you'll see something like this:(アップロードと処理には数分かかります...これらのファイルのいくつかは大きいファイルになります。アップロードが完了すると、次のような画面が表示されます。)

![](../.gitbook/assets/upload-counter-data-fully-loaded.png)

You can click on the download arrows to the far right of each file to see what we have stored. If you'd like to replace this data later you can click the Trash can to the right of the row and then upload a new file — your scenario forecasts will automatically recalculate to use the new data.(各ファイルの右端にあるダウンロード用の矢印をクリックすると、保存されているものを確認することができます。もし、このデータを後で交換したい場合は、行の右側にあるゴミ箱をクリックし、新しいファイルをアップロードしてください - シナリオ予測は自動的に新しいデータを使用して再計算されます。)

Note that because COUNTER files include Open Access journals, and journals that have stopped publishing, not all of the journals in your COUNTER files will appear in your Forecast dashboards. Furthermore, if you are missing price data, those journals will be missing even if they are currently publishing and have COUNTER usage ([see here to correct this](upload-title-prices.md)).(COUNTERファイルにはオープンアクセスジャーナルや出版中止のジャーナルが含まれているため、COUNTERファイル内のすべてのジャーナルが予測ダッシュボードに表示されるわけではないことにご注意ください。ジャーナルの価格データが不足している場合、それらのジャーナルは現在出版されていてCOUNTERの利用があったとしても、表示できません。（[see here to correct this(修正方法はこちら)](upload-title-prices.md))。)

\
